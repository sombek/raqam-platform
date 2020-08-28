<template>
	<div class="hello">
		<div class="container">
			<div class="border">
				<div class="zero">
					{{first}}
				</div>
				<div class="one">
					{{second}}
				</div>
			</div>
			<br>
			<div class="title">
				<h3>
					مرحبا بك في
				</h3>
				<h1>
					منصة رقم التقنية
				</h1>
			</div>

			<div class="services">
				<img src="../assets/computer.gif" height="200" alt="">
				<h2>ماذا نقدم؟</h2>

				<p style="text-align: right">
					تنقسم خدماتنا بشكل أساسي إلى قسمين: الخدمات الإستشارية و الخدمات التطويرية.
				</p>
				<p style="text-align: right">
					و عليها يتم العمل لتحديد المتطلبات الخاصة بالعميل ويتم تضمينها مثل الخدمات ادناه:
				</p>
				<ul>
					<li>
						تقديم الاستشارات المتعلقة بالمعمارية التقنية القائمة
					</li>
					<li>
						تشخيص و توضيح المخاطر التقنية للحلول التقنية القائمة
					</li>
					<li>
						تحليل و تطوير إجراءات الأعمال و وضع حلول رقمية
					</li>
					<li>
						تطوير، و تصميم، و تنفيذ الحلول التقنية الجديدة
					</li>
					<li>
						إستخدام التقنيات المتطورة للعمليات التقنية. مثل: الـ
						<span style="font-size:18pt;font-family: 'Pixelar Regular W01 Regular', serif;">
						DevOps
					</span>
					</li>

				</ul>

			</div>

			<div class="buttons">
				<div class="pixel2"
					 onclick="window.open('https://wa.me/966595585131/?text=%D9%85%D8%B1%D8%AD%D8%A8%D9%8B%D8%A7%D8%8C+%D8%A7%D8%B1%D9%8A%D8%AF+%D8%A7%D9%84%D8%A5%D8%B3%D8%AA%D9%81%D8%B3%D8%A7%D8%B1+%D8%B9%D9%86+%D8%AE%D8%AF%D9%85%D8%A7%D8%AA+%D9%85%D9%86%D8%B5%D8%A9+%D8%B1%D9%82%D9%85+%D8%A7%D9%84%D8%AA%D9%82%D9%86%D9%8A%D8%A9')">
					<p>
						الإستعلام عن خدماتنا
					</p>
				</div>
				<div class="pixel2" onclick="window.location.href = 'tel:0595585131'">
					<p>
						الإتصال بنا
					</p>
				</div>
			</div>
			<div class="footer">
				جميع الحقوق محفوظة 2020 ⓒ
			</div>
		</div>
	</div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        props: {
            msg: String
        },
        data() {
            return {
                first: 0,
                second: 1
            }
        },
        mounted() {
            window.setInterval(() => {
                this.toggleNumbers();
            }, 3000);

        },
        methods: {
            toggleNumbers() {
                this.first = !this.first ? 1 : 0;
                this.second = !this.second ? 1 : 0;
                setTimeout(() => this.first = this.first ? 1 : 0, 100)
                setTimeout(() => this.second = this.second ? 1 : 0, 500)
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.container {
		height: 100%;
		position: relative;
	}

	.hello {
		height: 100%;
		width: 100%;
		background-color: #ff6532;
		padding-top: 60px;
		display: inline-table;
	}

	.title {
		margin-bottom: 100px;
	}

	h1 {
		margin: unset;
		color: white;
		font-size: 92px;
		font-weight: 100;
	}

	h3 {
		margin: unset;
		color: white;
		font-weight: 100;
	}

	@media only screen and (max-width: 768px) {
		h1 {
			font-size: 12vw;
		}

		div.pixel2 {
			margin: 10px;
		}

		div.services {
			width: 90%;
		}
	}

	li:before {
		content: '*';
	}

	li {
		text-align: right;
		list-style: none;
	}

	.services {
		width: 60%;
		color: #eaecce;
		margin: auto auto 50px;
	}

	.buttons {
		height: 200px;
	}

	.services h2 {
		font-size: 32pt;
		font-weight: 100;
	}

	.border {
		height: 143px;
		width: 59px;
		border: 7px solid white;
		border-radius: 3px;
		margin: 0 auto;
		position: relative;
	}

	.zero, .one {
		font-family: "Pixelar Regular W01 Regular", serif !important;
		color: white;
		font-size: 66px;
	}

	.pixel2 p {
		margin: -7px 0 0;
	}

	.pixel2 {
		padding: 10px 10px;
		position: relative;
		background: white;

		z-index: 2;
		margin: auto 20px;
		font-size: 25px;
		color: #ff6532;

		display: inline-block;
		vertical-align: top;

		width: 250px;
		height: auto;

		cursor: pointer;

		-webkit-touch-callout: none;
		-webkit-user-select: none;
		-khtml-user-select: none;
		-moz-user-select: none;
		-ms-user-select: none;
		user-select: none;
	}

	.pixel2:active {
		top: 2px;
	}

	.pixel2::before {
		content: "";
		display: block;
		position: absolute;
		top: 10px;
		bottom: 10px;
		left: -10px;
		right: -10px;
		background: white;
		z-index: -1;
	}

	.pixel2::after {
		content: "";
		display: block;
		position: absolute;
		top: 4px;
		bottom: 4px;
		left: -6px;
		right: -6px;
		background: white;
		z-index: -1;
	}

	.footer {
		position: absolute;
		bottom: 5px;
		left: calc(50% - 105px);
	}

</style>
