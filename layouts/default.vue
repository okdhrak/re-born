<template>
	<div class="wrap">
		<header class="header">
			<h1><img src="~/assets/image/bnr_welcome.gif"></h1>
			<div class="marquee">
				<div class="marquee__inner">
					<img src="~/assets/image/angle.gif">ようこそ！<span>マイホームページ</span>へ！<img src="~/assets/image/angle.gif">
				</div>
			</div>
			<div class="headline">
				<p><img src="~/assets/image/counter.gif"></p>
				<p class="txt"><span>★Have a funny time.★</span></p>
				<p class="txt"><span>★USA!USA!★</span></p>
				<p><img src="~/assets/image/americanflag.gif"></p>
			</div>
			<p class="hb"><img src="~/assets/image/bnr_hb_1.gif"></p>
		</header>
		<hr>
		<nuxt />
		<hr>
		<footer class="footer">
			<div class="footer__cont">
				<p>【推奨環境】<br>ブラウザ：InternetExplorer6、Netscape3.0 推奨<br>(解像度：960*640 以上推奨)</p>
			</div>
			<ul class="footer__bnr">
				<li><img src="~/assets/image/bnr_ie.gif"></li>
				<li><img src="~/assets/image/bnr_ns.gif"></li>
				<li><img src="~/assets/image/bnr_hb_2.gif"></li>
				<li><img src="~/assets/image/bnr_notepad.gif" style="height: 31px;"></li>

			</ul>
			<div class="footer__copy">
				<p>2020 &copy; okdhrak</p>
			</div>
		</footer>
		<div class="totop">
			<nuxt-link v-scroll-to="'.wrap'" to><img src="~/assets/image/totop.gif"></nuxt-link>
		</div>
	</div>
</template>

<script>
export default {
	head: {
	},
	head () {
		return {
			title: 'マイホームページ 🚀',
			script: [
				{ src: 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js' }
			],
			link: [
				{ rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Roboto&display=swap' }
			]
		}
	},
}
</script>

<style lang="scss">
	html {
	font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
	font-size: 16px;
	word-spacing: 1px;
	-ms-text-size-adjust: 100%;
	-webkit-text-size-adjust: 100%;
	-moz-osx-font-smoothing: grayscale;
	-webkit-font-smoothing: antialiased;
	box-sizing: border-box;
}

*,
*:before,
*:after {
	box-sizing: border-box;
	margin: 0;
}
ul {
	list-style: none;
	margin: 0;
	padding: 0;
}

@keyframes blink_effect {
    0% {
        opacity: 0;
    }
	50% {
        opacity: 0;
    }
	51% {
        opacity: 1;
    }
    100% {
        opacity: 100;
    }
}
@keyframes marquee {
	0% {
	    left: 100%;
	    transform: translate(0);
	}
	100% {
	    left: 0;
	    transform: translate(-100%);
	}
}
.header {
	position: relative;
	padding: 0 0 20px;
	h1 {
		text-align: center;
	}
	.marquee {
		overflow: hidden;
		position: relative;
		height: 60px;
		background: #fff;
		.marquee__inner {
			position: absolute;
			top: 0;
			white-space: nowrap;
			animation-name: marquee;
			animation-timing-function: linear;
			animation-duration: 20s;
			animation-iteration-count: infinite;

			text-shadow: 1px 5px 0 #ff0000;
			font-style: oblique;
			font-size: 30px;
			font-weight: bold;
			span {
				animation: blink_effect .5s linear 0s infinite normal none running;
			}
			img {
				width: 70px;
			}
		}
	}
	.headline {
		text-align: center;
		padding: 30px 0 0;
		.txt {
			margin: 5px 0 0;
			span {
				background: brown;
				color: yellow;
			}
		}
	}
	.hb {
		position: absolute;
		top: 10px;
		left: 10px;
	}
}
.footer {
	text-align: center;
	padding: 30px;
	.footer__bnr {
		margin: 20px 0 0;
		li {
			display: inline-block;
		}
	}
	.footer__copy {
		margin: 20px 0 0;
	}
}
.totop {
	position: fixed;
	bottom: 20px;
	right: 20px;
}

@media (max-width: 420px) { // 420px以下に適用
.header {
	h1 {
		img {
			width: 50%;
		}
	}
	.marquee {
		height: 42px;
		.marquee__inner {
			font-size: 20px;
			img {
				width: 50px;
			}
		}
	}
	.headline {
		text-align: center;
		padding: 30px 0 0;
		.txt {
			margin: 5px 0 0;
			span {
				background: brown;
				color: yellow;
			}
		}
	}
}
}
</style>
