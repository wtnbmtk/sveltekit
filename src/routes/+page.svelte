<script>
	import logo_webp from '$lib/assets/logo1.webp';
	import logo_png from '$lib/assets/logo1.png';
	import draw_webp from '$lib/assets/draw.webp';
	import draw_png from '$lib/assets/draw.png';
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
			</div>
			<div class="image">
				<picture>
					<source srcset={draw_webp} type="image/webp" />
					<img src={draw_png} alt="logo" width="auto" height="500" />
				</picture>
			</div>
		</div>
	</section>
	<section id="summary" class="contents contentsCenter">
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
		<div>
			<h4>シンプルプラン</h4>
			<dl class="DataGrid">
				<dt>プラン名</dt>
				<dd>シンプルプラン</dd>
				<dt>基本制作費と構成</dt>
				<dd><b>40,000円~</b>でトップページ、子ページ(2ページまで)を制作</dd>
				<dt>運営費</dt>
				<dd>
					ウェブダチでの管理費2,000円/月+ドメイン利用料+Cloudflare Pages<span>*1</span>の<a
						class="prices"
						href="https://pages.cloudflare.com/#pricing"
						target="_blank">利用料</a
					>
				</dd>
				<dt>ページ追加費</dt>
				<dd>A4サイズ1ページで10,000円</dd>
			</dl>
			<h4>CMS実装プラン</h4>
			<dl class="DataGrid">
				<dt>プラン名</dt>
				<dd>CMS実装プラン</dd>
				<dt>基本制作費と構成</dt>
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
					>+Newt<span>*2</span>の<a class="prices" href="https://www.newt.so/plan" target="_blank"
						>利用料</a
					>
				</dd>
				<dt>ページ追加費</dt>
				<dd>A4サイズ1ページで20,000円</dd>
			</dl>

			<p>*価格は全て税込価格です。</p>
			<p>*1 Cloudflare PagesはCloudflare, Inc.が提供するホスティングサービスです。</p>
			<p>*2 NewtはNewt株式会社が提供するCMSサービスです。</p>
		</div>
	</section>
</main>
