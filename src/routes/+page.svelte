<script>
	import draw_small from '$lib/assets/draw_small.png';
	import draw_medium from '$lib/assets/draw_medium.png';
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
					<source srcset={draw_small} media="(max-width: 1200px)" />
					<img src={draw_medium} alt="logo" width="533" height="400" />
				</picture>
			</div>
		</div>
	</section>
	<section id="summary" class="contents contentsCenter">
		<script async src="https://js.stripe.com/v3/buy-button.js">
		</script>

		<stripe-buy-button
			buy-button-id="buy_btn_1O4Iw7JXSEtNpSmgsWNS1KD6"
			publishable-key="pk_test_51O4HsoJXSEtNpSmgsUNyvBZIbXQx9N9REkzZeTdK8tS29sFxvzG9dmRRyHK8gasucWWpbbZZRrbzrMjVlYdcZS9w00pbBQHnhM"
		/>
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

		<h4>シンプルプラン</h4>
		<dl class="DataGrid">
			<dt>プラン名</dt>
			<dd>シンプルプラン</dd>
			<dt>基本制作費と構成</dt>
			<dd><b>40,000円~</b>でトップページ、子ページ(2ページまで)を制作</dd>
			<dt>運営費</dt>
			<dd>
				<ul>
					<li>
						ドメインサービス(例:Xserverドメイン)の<a
							class="prices"
							href="https://www.xdomain.ne.jp/"
							target="_blank">利用料</a
						>
					</li>
					<li>
						ホスティングサービス(例:Cloudflare Pages)<span>*1</span>の<a
							class="prices"
							href="https://pages.cloudflare.com/#pricing"
							target="_blank">利用料</a
						>
					</li>
				</ul>
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
				<ul>
					<li>
						ドメインサービス(例:Xserverドメイン)の<a
							class="prices"
							href="https://www.xdomain.ne.jp/"
							target="_blank">利用料</a
						>
					</li>
					<li>
						ホスティングサービス(例:Cloudflare Pages)<span>*1</span>の<a
							class="prices"
							href="https://pages.cloudflare.com/#pricing"
							target="_blank">利用料</a
						>
					</li>
					<li>
						CMSサービス(例:Spearly CMS)<span>*2</span>の<a
							class="prices"
							href="https://spearly.com/ja/cms/pricing"
							target="_blank">利用料</a
						>
					</li>
				</ul>
			</dd>
			<dt>ページ追加費</dt>
			<dd>A4サイズ1ページで20,000円</dd>
		</dl>
		<div class="small_text">
			<p>*価格は全て税込価格です。</p>
			<p>*1 Cloudflare PagesはCloudflare, Inc.が提供するホスティングサービスです。</p>
			<p>*2 NewtはNewt株式会社が提供するCMSサービスです。</p>
		</div>
	</section>
</main>

<style>
	.DataGrid dt:nth-of-type(4) {
		border-bottom: solid 1px black;
	}
	.DataGrid dd:nth-of-type(4) {
		border-bottom: solid 1px black;
	}
	.small_text {
		font-size: small;
		margin-bottom: 0;
	}
</style>
