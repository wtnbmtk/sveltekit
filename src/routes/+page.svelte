<script>
	import logo from '$lib/assets/logo1.svg';
	import profile from '$lib/assets/profile.jpeg';
</script>

<main>
	<section id="TopView" class="contents">
		<div class="TopContents">
			<div class="text">
				<hgroup>
					<h2>繋がるWebクリエイティブパートナー</h2>
					<p>
						ウェブダチは生産性を高めたWebクリエイティブで、サポートのリソースを増やしたサイト運営を行います。
					</p>
				</hgroup>
				<a class="line" href="https://lin.ee/VTOX579"
					><img
						src="https://scdn.line-apps.com/n/line_add_friends/btn/ja.png"
						alt="友だち追加"
						height="36"
						border="0"
					/></a
				>
			</div>
			<div class="image">
				<img alt="logo" src={logo} />
			</div>
		</div>
	</section>
	<section id="summary" class="contents">
		<h3>VISION</h3>
		<p>
			現代では対話型AIなどの様々な便利なテクノロジーの登場により、創造するプロセスの効率化は格段に向上しています。テクノロジーを駆使した効率的なクリエイティブは、ビジネスにおいてクリエイターとクライアントとの繋がりを強化します。ウェブダチは人々がお互いを思い遣り、助け合うことで生まれるクリエイティブを思い描いています。
		</p>
		<h3>WORKFLOW</h3>
		<ol>
			<li>LINE公式アカウントに相談を受け付け</li>
			<li>サイトデザインについてヒアリング</li>
			<li>コーディング作業</li>
			<li>サイトを公開</li>
			<li>継続的にサイト運営をサポート</li>
		</ol>
		<h3>PRICES&DETAILS</h3>
		<p>お支払い頂く料金はプランによって異なり、以下に示す各費用の合算となります。</p>
		<div class="DataGrid">
			<dl>
				<dt>プラン名</dt>
				<dd>シンプルプラン</dd>
				<dd>CMS実装プラン</dd>
				<dt>基本制作費と構成</dt>
				<dd><b>40,000円~</b>でトップページ、子ページ(2ページまで)を制作</dd>
				<dd>
					<b>140,000円~</b
					>でトップページ(記事一覧含む)、子ページ(記事本文、各カテゴリーの一覧、各年の一覧、各著者の記事一覧、検索結果一覧)を制作
				</dd>
				<dt>運営費</dt>
				<dd>
					ウェブダチでの管理費2,000円/月+ドメイン利用料+Cloudflare Pages<span>*1</span>の<a
						class="prices"
						href="https://pages.cloudflare.com/#pricing"
						target="_blank">利用料</a
					>
				</dd>
				<dd>
					ウェブダチでの管理費2,000円/月+ドメイン利用料+Cloudflare Pages<span>*1</span>の<a
						class="prices"
						href="https://pages.cloudflare.com/#pricing"
						target="_blank">利用料</a
					>+Newt<span>*2</span>の<a class="prices" href="https://www.newt.so/plan" target="_blank"
						>利用料</a
					>
				</dd>
				<dt>ページ追加費</dt>
				<dd>A4サイズ1ページで10,000円</dd>
				<dd>A4サイズ1ページで20,000円</dd>
			</dl>
			<p>*価格は全て税込価格です。</p>
			<p>*1 Cloudflare PagesはCloudflare, Inc.が提供するホスティングサービスです。</p>
			<p>*2 NewtはNewt株式会社が提供するCMSサービスです。</p>
		</div>
	</section>
	<section id="profile" class="contents">
		<div>
			<h3>PROFILE</h3>
			<div class="image">
				<img alt="profile" src={profile} />
			</div>
			<div class="text">
				<h3>モトキ</h3>
				<p>
					東京工芸大学卒。同大学在学中にWeb開発のスキルを身に付け始める。現在では、HTML、CSS、JavaScriptをはじめ、Next.jsやGitなどのスキルを身に付け、効率的なWeb開発を得意としている。また、UI/UXデザインやSEOの知識を持っており、ユーザーが使いやすく、魅力的なWebサイト制作が行える。実績としては制作依頼を通して実践的なWeb開発の経験を積んでおり、ユーザーファーストな開発で評価されてきた。
				</p>
			</div>
		</div>
	</section>
	<section id="contact" class="contents">
		<div>
			<h3>CONTACT</h3>
			<!-- svelte-ignore a11y-missing-attribute -->
			<iframe
				id="form"
				style="border: none; width: 100%"
				height="691px"
				src="https://www.noway-form.com/ja/f/9b90dc54-ca75-4bf9-83ea-cf7dfe43908b/embed"
			/>
		</div>
	</section>
</main>

<style>
	main {
		container: main / inline-size;
		background-color: white;
		margin: 50px 0 0 0;
	}
	.contents {
		margin: auto;
		font-size: medium;
	}
	.contents::before {
		content: ' ';
		display: block;
		visibility: hidden;
	}
	.contents p {
		text-align: justify;
	}
	#TopView:before {
		margin-top: -100px;
		height: 100px;
	}
	#TopView {
		background: linear-gradient(220.55deg, #a531dc 0%, #4300b1 100%);
	}
	.TopContents {
		display: grid;
		place-content: center;
	}
	.TopContents div {
		display: grid;
		place-content: center;
		width: 100%;
		height: 250px;
		padding: 0 2rem;
	}
	.TopContents .text {
		color: white;
	}
	.TopContents .text h2 {
		margin-top: 0;
	}
	.TopContents .text a {
		display: contents;
	}
	.image img {
		margin: auto;
	}
	/* .TopContents .image {
  background: url(images/bg3.png) center;
} */
	.TopContents .image img {
		max-width: 250px;
	}
	.contents:nth-child(n + 2)::before {
		margin-top: -50px;
		height: 50px;
	}
	.contents:nth-child(n + 2) {
		padding: 0 1rem;
	}
	.contents:nth-child(n + 2) h2 {
		text-align: center;
	}
	.contents:nth-child(n + 2) h3 {
		text-align: center;
	}

	.DataGrid p {
		margin-top: 0;
	}
	.DataGrid dl {
		display: grid;
		grid-template-columns: 1fr 2fr 2fr;
		border-right: solid 1px black;
		border-left: solid 1px black;
		margin-bottom: 0;
	}
	.DataGrid dt {
		border-top: solid 1px black;
		background-color: blueviolet;
		color: white;
	}
	.DataGrid dt:nth-of-type(4) {
		border-bottom: solid 1px black;
	}
	.DataGrid dd {
		margin: 0;
		border-top: solid 1px black;
		border-left: solid 1px black;
		padding-left: 1rem;
	}
	.DataGrid dd:nth-of-type(7),
	.DataGrid dd:nth-of-type(8) {
		border-bottom: solid 1px black;
	}
	.DataGrid span {
		font-size: x-small;
		vertical-align: top;
	}
	.DataGrid p {
		font-size: small;
		margin-bottom: 0;
	}
	.prices {
		text-decoration: underline;
		color: blue;
	}
	#profile .image img {
		max-width: 80px;
		border-radius: 50%;
	}
	#profile .text {
		max-width: 400px;
		margin: auto;
	}
	#profile .text h3 {
		text-align: center;
	}
	#form h1 {
		display: none;
	}
	.FormGrid {
		display: grid;
		grid-template-columns: 1fr;
	}
	.gridGallery {
		display: grid;
		grid-gap: 1rem;
		place-content: center;
		grid-template-columns: 1fr 1fr;
	}
	.item {
		display: block;
		position: relative;
		width: 130px;
		overflow: hidden;
		margin: 0 auto;
	}
	.item::before {
		content: '';
		display: block;
		padding-top: 100%;
	}
	.item img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		right: 0;
		bottom: 0;
		left: 0;
		margin: auto;
		object-fit: cover;
		vertical-align: bottom;
		-webkit-transition: 0.3s ease-in-out;
		transition: 0.3s ease-in-out;
		-webkit-transform: scale(1);
		transform: scale(1);
	}
	.item:hover img {
		cursor: pointer;
		-webkit-transform: scale(1.3);
		transform: scale(1.3);
	}
	.lum-lightbox {
		top: 50px;
	}
	#gMap {
		display: block;
		width: 100%;
		height: 300px;
	}
	#content {
		width: 100%;
		height: 200px;
	}
	#spearly-list-body {
		margin: 0;
		padding: 0;
	}
	#spearly-list-body li {
		margin: 1rem auto;
	}
	#spearly-list-body li:first-child {
		margin-top: 0;
	}
	#spearly-list-body li:last-child {
		margin-bottom: 0;
	}
	#spearly-list-body a {
		display: block;
		color: lavender;
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
		position: relative;
		top: 0;
	}
	#spearly-list-body a:hover {
		top: -5px;
		transition: 0.3s ease-in-out;
	}
	#spearly-list-body a img {
		width: 100%;
		height: 130px;
		object-fit: cover;
	}
	#spearly-list-body a .articleTextLink {
		width: 100%;
		height: 130px;
		margin: 0;
		padding: 1rem;
	}
	.articleTextLink h3,
	.articleTextLink p {
		margin: 0;
	}
	.article-item-wrapper img {
		display: block;
		margin: 0 auto;
		height: 260px;
		object-fit: cover;
	}
</style>
