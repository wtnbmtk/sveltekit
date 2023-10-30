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
			<li>Slackワークスペースに招待</li>
			<li>サイトデザインについてヒアリング</li>
			<li>初期費用の入金確認後、制作を開始</li>
			<li>お客様にサイトをご確認していただき、運用を開始</li>
			<li>継続的にサイト運営をサポート</li>
		</ol>
		<h3>PRICES&DETAILS</h3>
		<p>
			お支払い頂く料金はプランによって異なり、以下に示す費用内訳の料金の合算となります。初期費用以外の各種サービスの料金はサイトの規模によって変動しますのでご注意ください。
		</p>

		<h4>Standard Plan</h4>
		<div class="plan">
			<dl class="data">
				<dt>プラン名</dt>
				<dd>Standard Plan</dd>
				<dt>初月支払総額</dt>
				<dd>￥50,000~</dd>
				<dt>内訳</dt>
				<dd>
					<ul>
						<li>初期費用<b>￥50,000</b></li>
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
				<dt>仕様</dt>
				<dd>
					基本となるA4サイズのページ（トップページやプロフィールページなど）が３ページまでで、CMS機能が無いスタンダードなプラン。
				</dd>
			</dl>
			<div class="stripe">
				<script async src="https://js.stripe.com/v3/buy-button.js">
				</script>

				<stripe-buy-button
					buy-button-id="buy_btn_1O5Ko4AIPjnW5yZ1LdZTGUDM"
					publishable-key="pk_live_51O4Nt8AIPjnW5yZ1xpcThU3EhrRdaLkVHN9YDM0otNAgKHrVoUwdLyZD7BHzJ1FvsFm7QoG2L2nn8kpEz2bsKLV000CU0ShlND"
				/>
			</div>
		</div>
		<h4>CMS Plan</h4>
		<div class="plan">
			<dl class="data">
				<dt>プラン名</dt>
				<dd>CMS Plan</dd>
				<dt>初月支払総額</dt>
				<dd>￥100,000~</dd>
				<dt>内訳</dt>
				<dd>
					<ul>
						<li>初期費用<b>￥100,000</b></li>
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
				<dt>仕様</dt>
				<dd>
					基本となるA4サイズのページ（トップページやブログ一覧など）が５ページまでで、CMS機能が付いたプラン。
				</dd>
			</dl>
			<div class="stripe">
				<script async src="https://js.stripe.com/v3/buy-button.js">
				</script>

				<stripe-buy-button
					buy-button-id="buy_btn_1O5gGSAIPjnW5yZ1wSW6KWxa"
					publishable-key="pk_live_51O4Nt8AIPjnW5yZ1xpcThU3EhrRdaLkVHN9YDM0otNAgKHrVoUwdLyZD7BHzJ1FvsFm7QoG2L2nn8kpEz2bsKLV000CU0ShlND"
				/>
			</div>
		</div>
		<h4>EC Plan</h4>
		<div class="plan">
			<dl class="data">
				<dt>プラン名</dt>
				<dd>EC Plan</dd>
				<dt>初月支払総額</dt>
				<dd>￥300,000~</dd>
				<dt>内訳</dt>
				<dd>
					<ul>
						<li>初期費用<b>￥300,000</b></li>
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
				<dt>仕様</dt>
				<dd>
					基本となるA4サイズのページ（トップページやブログ一覧など）が５ページまでで、CMSとEC機能が付いたプラン。
				</dd>
			</dl>
			<div class="stripe">
				<script async src="https://js.stripe.com/v3/buy-button.js">
				</script>

				<stripe-buy-button
					buy-button-id="buy_btn_1O6va2AIPjnW5yZ1N3wRK47m"
					publishable-key="pk_live_51O4Nt8AIPjnW5yZ1xpcThU3EhrRdaLkVHN9YDM0otNAgKHrVoUwdLyZD7BHzJ1FvsFm7QoG2L2nn8kpEz2bsKLV000CU0ShlND"
				/>
			</div>
		</div>
		<div class="small_text">
			<p>*価格は全て税込価格です。</p>
		</div>
	</section>
</main>

<style>
	.data {
		display: grid;
		grid-template-columns: 80px auto;
		border-right: solid 1px black;
		border-left: solid 1px black;
	}
	.data dt:nth-of-type(4) {
		border-bottom: solid 1px black;
	}
	.data dd:nth-of-type(4) {
		border-bottom: solid 1px black;
	}
	.data dd:nth-of-type(2) {
		font-size: 2rem;
	}
	.small_text {
		font-size: small;
		margin-bottom: 0;
	}
	.plan {
		display: grid;
		grid-template-columns: 2fr 1fr;
	}
	.stripe {
		width: max-content;
		display: grid;
		place-content: center;
		margin-left: 8px;
	}
	@media (width <= 800px) {
		.plan {
			display: initial;
		}
		.stripe {
			margin: 8px auto;
		}
	}
</style>
