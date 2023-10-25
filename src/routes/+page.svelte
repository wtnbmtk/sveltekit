<script>
	import draw_small from '$lib/assets/draw_small.png';
	import draw_medium from '$lib/assets/draw_medium.png';
</script>

<main>
	<section id="TopView" class="contents contentsTop">
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
		<h3>VISION</h3>
		<p>
			現代では対話型AIなどの様々な便利なテクノロジーの登場により、創造するプロセスの効率化は格段に向上しています。テクノロジーを駆使した効率的なクリエイティブは、ビジネスにおいてクリエイターとクライアントとの繋がりを強化します。ウェブダチは人々がお互いを思い遣り、助け合うことで生まれるクリエイティブを思い描いています。
		</p>
		<h3>WORKFLOW</h3>
		<ol>
			<li>LINE公式アカウントに相談を受け付け</li>
			<li>サイトデザインについてヒアリング</li>
			<li>基本制作費用の入金確認後、制作を開始</li>
			<li>お客様にサイトをご確認していただき、運用を開始</li>
			<li>継続的にサイト運営をサポート</li>
		</ol>
		<h3>PRICES&DETAILS</h3>
		<p>
			お支払い頂く料金はプランによって異なり、以下に示す費用欄内の料金の合算となります。基本制作費用以外の各種サービスの料金はサイトの規模によって変動しますのでご注意ください。
		</p>

		<h4>Webdachi S</h4>
		<dl class="DataGrid">
			<dt>プラン名</dt>
			<dd>Webdachi S</dd>
			<dt>構成</dt>
			<dd>
				基本となるA4サイズのページ（トップページやプロフィールページなど）が３ページまでで、CMS機能が無いスタンダードなプラン。
			</dd>
			<dt>費用</dt>
			<dd>
				<ul>
					<li>基本制作費用<b>￥50,000</b></li>
					<li>
						ドメインサービス（例 : Xserverドメイン）の<a
							class="prices"
							href="https://www.xdomain.ne.jp/"
							target="_blank">利用料</a
						>
					</li>
					<li>
						ホスティングサービス（Cloudflare Pages）の<a
							class="prices"
							href="https://pages.cloudflare.com/#pricing"
							target="_blank">利用料</a
						>
					</li>
				</ul>
			</dd>
		</dl>
		<h4>Webdachi CMS</h4>
		<dl class="DataGrid">
			<dt>プラン名</dt>
			<dd>Webdachi CMS</dd>
			<dt>構成</dt>
			<dd>
				基本となるA4サイズのページ（トップページやブログ一覧など）が５ページまでで、CMS機能が付いたプラン。
			</dd>
			<dt>費用</dt>
			<dd>
				<ul>
					<li>基本制作費用<b>￥100,000</b></li>
					<li>
						ドメインサービス（例 : Xserverドメイン）の<a
							class="prices"
							href="https://www.xdomain.ne.jp/"
							target="_blank">利用料</a
						>
					</li>
					<li>
						ホスティングサービス（Cloudflare Pages）の<a
							class="prices"
							href="https://pages.cloudflare.com/#pricing"
							target="_blank">利用料</a
						>
					</li>
					<li>
						CMSサービス（Spearly CMS）の<a
							class="prices"
							href="https://spearly.com/ja/cms/pricing"
							target="_blank">利用料</a
						>
					</li>
				</ul>
			</dd>
		</dl>
		<h4>Webdachi EC</h4>
		<dl class="DataGrid">
			<dt>プラン名</dt>
			<dd>Webdachi EC</dd>
			<dt>構成</dt>
			<dd>
				基本となるA4サイズのページ（トップページやブログ一覧など）が５ページまでで、CMSとEC機能が付いたプラン。
			</dd>
			<dt>費用</dt>
			<dd>
				<ul>
					<li>基本制作費用<b>￥200,000</b></li>
					<li>
						ドメインサービス（例 : Xserverドメイン）の<a
							class="prices"
							href="https://www.xdomain.ne.jp/"
							target="_blank">利用料</a
						>
					</li>
					<li>
						ホスティングサービス（Cloudflare Pages）の<a
							class="prices"
							href="https://pages.cloudflare.com/#pricing"
							target="_blank">利用料</a
						>
					</li>
					<li>
						CMSサービス（Spearly CMS）の<a
							class="prices"
							href="https://spearly.com/ja/cms/pricing"
							target="_blank">利用料</a
						>
					</li>
					<li>
						決済サービス（Stripe）の<a
							class="prices"
							href="https://stripe.com/jp/pricing"
							target="_blank">利用料</a
						>
					</li>
				</ul>
			</dd>
		</dl>
		<div class="small_text">
			<p>*価格は全て税込価格です。</p>
		</div>
		<div class="stripe">
			<div>
				<script async src="https://js.stripe.com/v3/buy-button.js">
				</script>

				<stripe-buy-button
					buy-button-id="buy_btn_1O5760AIPjnW5yZ1u66AH6Qq"
					publishable-key="pk_test_51O4Nt8AIPjnW5yZ1KjthGtKH1YumfWSYbezFmURu3BbnG56FQdD93gBkcNZFfdG3eoiK8IovHplNg0gT30DnuNMF00IFrLsMbL"
				/>
			</div>
			<div>
				<script async src="https://js.stripe.com/v3/buy-button.js">
				</script>

				<stripe-buy-button
					buy-button-id="buy_btn_1O58onAIPjnW5yZ1ihJAzbnx"
					publishable-key="pk_test_51O4Nt8AIPjnW5yZ1KjthGtKH1YumfWSYbezFmURu3BbnG56FQdD93gBkcNZFfdG3eoiK8IovHplNg0gT30DnuNMF00IFrLsMbL"
				/>
			</div>
			<div>
				<script async src="https://js.stripe.com/v3/buy-button.js">
				</script>

				<stripe-buy-button
					buy-button-id="buy_btn_1O58uMAIPjnW5yZ1DH60VntI"
					publishable-key="pk_test_51O4Nt8AIPjnW5yZ1KjthGtKH1YumfWSYbezFmURu3BbnG56FQdD93gBkcNZFfdG3eoiK8IovHplNg0gT30DnuNMF00IFrLsMbL"
				/>
			</div>
		</div>
	</section>
</main>

<style>
	.DataGrid dt:nth-of-type(3) {
		border-bottom: solid 1px black;
	}
	.DataGrid dd:nth-of-type(3) {
		border-bottom: solid 1px black;
	}
	.small_text {
		font-size: small;
		margin-bottom: 0;
	}
	.stripe {
		display: grid;
		margin: 16px auto;
	}
	.stripe div {
		margin: 8px auto;
	}
	@container main (min-width: 800px) {
		.stripe {
			grid-template-columns: 1fr 1fr;
		}
	}
</style>
