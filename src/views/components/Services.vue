<template>
	<div class="services">
		<img src="../../assets/computer.gif" height="200" alt="">
		<h2>ماذا نقدم؟</h2>

		<div class="text">

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

	</div>
</template>
<script>
	export default {
		name: 'Services'
	}
</script>
<style scoped>
	.services {
		width: 60%;
		color: #eaecce;
		margin: auto auto 50px;
	}

	h2 {
		font-size: 32pt;
		font-weight: 100;
		margin-top: 0;
	}

	@media only screen and (max-width: 768px) {
		div.services {
			width: 90%;
		}

		div.text {
			width: 100%;
		}
	}

	.text {
		width: 70%;
		margin: auto;
	}

	li:before {
		content: '*';
	}

	li {
		text-align: right;
		list-style: none;
	}

</style>
