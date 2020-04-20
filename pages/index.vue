<template>
	<div class="container">
		<!--<h1>{{title}}</h1>
		<p><img src="../assets/image/person_1.gif" style="width: 142px;"></p>
		<p><img src="~/assets/image/bg_3.gif"></p>
		<p><img src="/re-born/image/bg_3.gif"></p>-->

		<section class="lead">
			<h2>ホームページづくりのことならお任せください。</h2>
			<p>近未来を感じさせる、クールでイカしたホームページデザインが得意です。<br>ボームページの作成、リニューアルをお考えの企業様はお気軽にご相談ください！<br>個人店舗・事業主のポームページもお任せください。</p>
			<p><img src="~/assets/image/laptop.gif"><img src="~/assets/image/player_1.gif" style="width: 100px;"><img src="~/assets/image/laptop.gif"><img src="~/assets/image/player_2.gif" style="width: 100px;"><img src="~/assets/image/laptop.gif"></p>

		</section>
		<section class="info">
			<h2><img src="~/assets/image/ttl_info.gif">お知らせ</h2>
			<ul>
				<li><img src="~/assets/image/icon_hot.gif">2020年4月1日ホームページをリニューアルしました。(リニューアル前のサイトは<a href="https://okdhrak.github.io/" target="_blank">こちら</a>)</li>
			</ul>
			<p class="line"><img src="~/assets/image/line_2.gif"></p>
		</section>
		<section class="skill">
			<h2><img src="~/assets/image/ttl_skill.gif">スキル</h2>
			<table border="1" cellspacing="2" cellpadding="10">
				<tr>
					<th>okdhrak</th>
					<td><img src="~/assets/image/guiterlist.gif"></td>
				</tr>
				<tr>
					<th>HTML5</th>
					<td>★★★★★</td>
				</tr>
				<tr>
					<th>CSS3</th>
					<td>★★★★★</td>
				</tr>
				<tr>
					<th>JavaScript</th>
					<td>★★★★★</td>
				</tr>
				<tr>
					<th>PHP</th>
					<td>★★★★★</td>
				</tr>
			</table>
			<p class="skill__note">[ DB ] MySQL / SQLite<br>[ ライブラリ、フレームワーク ] Compass / jQuery / Vue / CakePHP / WordPress / Smarty / PEAR<br>[ ソフトウェア、サービス ] Microsoft Excel / Illustrator / Photoshop / Dreamweaver / Atom / ネクストエンジン / AWS</p>
			<p class="line"><img src="~/assets/image/line_2.gif"></p>
		</section>
		<section class="work">
			<h2><img src="~/assets/image/ttl_case.gif">事例</h2>
			<table border="1" cellspacing="2" cellpadding="10">
				<tr>
					<th>不動産販売ポータルサイト</th>
					<td><nuxt-link to="/work_1">サイトを表示</nuxt-link></td>
				</tr>
				<tr>
					<th>建築会社コーポレートサイト</th>
					<td><nuxt-link to="/work_2">サイトを表示</nuxt-link></td>
				</tr>
				<tr>
					<th>リノベーションポータル</th>
					<td><nuxt-link to="/work_3">サイトを表示</nuxt-link></td>
				</tr>
			</table>
		</section>
		<section class="link">
			<h3>リンク集</h3>
			<ul>
				<li><a href="https://www.kantei.go.jp/" target="_blank"><img src="~/assets/image/logo_kantei.png"></a></li>
				<li><a href="http://www.kcna.kp/kcna.user.home.retrieveHomeInfoList.kcmsf" target="_blank"><img src="~/assets/image/logo_kitacho.jpg"></a></li>
				<li><a href="https://www.whitehouse.gov/" target="_blank"><img src="~/assets/image/logo_whitehouse.png"></a></li>
				<li><a href="https://www.mea.gov.in/" target="_blank"><img src="~/assets/image/logo_india.png" style="width: 100px;"></a></li>
			</ul>
		</section>
	</div>
</template>


<script>
export default {
	head: {
	},
	head () {
		return {
			//title: '俺のホームページ 🚀',
		}
	},
	data: function(){
		return {
			title: '俺のホームページ',
			message: 'this is message.',
		};
	},
};
</script>

<style>
/*@import "../assets/common.css";*/
</style>

<style lang="scss">
body {
	background: url('../assets/image/bg_1.gif');
	/*background: url('/re-born/image/bg_1.gif');*/

}

.container {
	section {
		padding: 30px 0;
		text-align: center;
		h2 {
			padding: 0 0 20px;
			font-style: oblique;
		}
		.line {
			margin: 50px 0 0;
		}
		&.lead {
			background: url('../assets/image/bg_3.gif');
		}
		&.skill {
			table {
				margin: 0 auto;
				width: 500px;
				tr {
					th {
						width: 60%;
						background: blue;
						color: white;
					}
					td {
						width: 40%;
						background: white;
					}
				}
			}
			.skill__note {
				font-size: 14px;
				margin: 30px 0 0;
			}
		}
		&.work {
			table {
				margin: 0 auto;
				width: 500px;
				tr {
					th {
						width: 40%;
						background: green;
						color: white;
					}
					td {
						width: 60%;
						background: white;
					}
				}
			}
		}
		&.link {
			background: url('../assets/image/bg_5.gif');
		}
	}

}

.info {
	a {
		font-style: oblique;
	}
}

@media (max-width: 420px) { // 420px以下に適用
.container {
	section {
		padding: 20px 0;
		h2 {
		}
		.line {
			margin: 30px 0 0;
			img {
				width: 100%;
			}
		}
		&.lead {
			background: url('../assets/image/bg_3.gif');
		}
		&.skill {
			table {
				margin: 0 2%;
				width: 96%;
				tr {
					th {
						width: 100%;
						display: inline-block;
					}
					td {
						width: 100%;
						display: inline-block;
					}
				}
			}
			.skill__note {
				font-size: 13px;
				margin: 20px 0 0;
			}
		}
		&.work {
			table {
				margin: 0 2%;
				width: 96%;
				tr {
					th {
						width: 100%;
						display: inline-block;
					}
					td {
						width: 100%;
						display: inline-block;
					}
				}
			}
			.skill__note {
				font-size: 13px;
				margin: 20px 0 0;
			}
		}
	}
}
}
</style>
