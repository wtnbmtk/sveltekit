<script>
	import profile_webp from '$lib/assets/profile.webp';
	import profile_jpg from '$lib/assets/profile.jpg';
</script>

<main>
	<section id="about" class="contents contentsTop contentsCenter">
		<h3>ABOUT</h3>
		<div class="image">
			<picture>
				<source srcset={profile_webp} type="image/webp" />
				<img src={profile_jpg} alt="profile" />
			</picture>
		</div>
		<div class="text">
			<h4>Webエンジニア：モトキ</h4>
			<p>
				東京工芸大学卒。同大学在学中にWeb開発のスキルを身に付け始める。現在では、HTML、CSS、JavaScriptをはじめ、Next.jsやGitなどのスキルを身に付け、効率的なWeb開発を得意としている。また、UI/UXデザインやSEOの知識を持っており、ユーザーが使いやすく、魅力的なWebサイト制作が行える。実績としては制作依頼を通して実践的なWeb開発の経験を積んでおり、ユーザーファーストな開発で評価されてきた。
			</p>
		</div>
	</section>
</main>

<style>
	#about .image img {
		max-width: 80px;
		border-radius: 50%;
		margin: auto;
	}
	#about .text {
		max-width: 400px;
		margin: auto;
	}
	#about .text h4 {
		text-align: center;
	}
</style>
