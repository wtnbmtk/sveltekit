<script>
	import draw_medium from '$lib/assets/dachi-m.png';
	import draw_small from '$lib/assets/dachi-s.png';
	import plan_Standard from '$lib/assets/Standard.png';
	import plan_CMS from '$lib/assets/CMS.png';
	import plan_EC from '$lib/assets/EC.png';
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
					<source srcset={draw_medium} media="(min-width: 1200px)" />
					<img src={draw_small} alt="draw" width="517" height="400" />
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
			<li>製作費の入金確認後、制作を開始</li>
			<li>お客様にサイトをご確認していただき、運用を開始</li>
			<li>継続的にサイト運営をサポート</li>
		</ol>
		<h3>PRICES&DETAILS</h3>
		<p>
			お支払い頂く料金はプランによって異なり、以下に示す費用内訳の料金の合算となります。製作費以外の各種サービスの料金はサイトの規模によって変動しますのでご注意ください。価格は全て税込価格です。
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
						<li>製作費<b>￥50,000</b>（初期費用）</li>
						<li>ドメインサービスの利用料</li>
						<li>ホスティングサービスの利用料（従量課金）</li>
					</ul>
				</dd>
				<dt>仕様</dt>
				<dd>
					<ul>
						<li>オリジナルデザイン</li>
						<li>固定ページA4サイズ3ページまで</li>
						<li>独自ドメイン</li>
						<li>サーバーレス</li>
					</ul>
				</dd>
			</dl>
			<div class="stripe">
				<div class="catalog">
					<img src={plan_Standard} alt="plan" width="288" height="288" />
					<script async src="https://js.stripe.com/v3/buy-button.js">
					</script>

					<stripe-buy-button
						buy-button-id="buy_btn_1O5Ko4AIPjnW5yZ1LdZTGUDM"
						publishable-key="pk_live_51O4Nt8AIPjnW5yZ1xpcThU3EhrRdaLkVHN9YDM0otNAgKHrVoUwdLyZD7BHzJ1FvsFm7QoG2L2nn8kpEz2bsKLV000CU0ShlND"
					/>
				</div>
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
						<li>製作費<b>￥100,000</b>（初期費用）</li>
						<li>ドメインサービスの利用料</li>
						<li>ホスティングサービスの利用料（従量課金）</li>
						<li>CMSサービスの利用料（月額費用）</li>
					</ul>
				</dd>
				<dt>仕様</dt>
				<dd>
					<ul>
						<li>オリジナルデザイン</li>
						<li>固定ページA4サイズ5ページまで</li>
						<li>独自ドメイン</li>
						<li>サーバーレス</li>
						<li>ヘッドレスCMS</li>
					</ul>
				</dd>
			</dl>
			<div class="stripe">
				<div class="catalog">
					<img src={plan_CMS} alt="plan" width="288" height="288" />
					<script async src="https://js.stripe.com/v3/buy-button.js">
					</script>

					<stripe-buy-button
						buy-button-id="buy_btn_1O5gGSAIPjnW5yZ1wSW6KWxa"
						publishable-key="pk_live_51O4Nt8AIPjnW5yZ1xpcThU3EhrRdaLkVHN9YDM0otNAgKHrVoUwdLyZD7BHzJ1FvsFm7QoG2L2nn8kpEz2bsKLV000CU0ShlND"
					/>
				</div>
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
						<li>製作費<b>￥300,000</b>（初期費用）</li>
						<li>ドメインサービスの利用料</li>
						<li>ホスティングサービスの利用料（従量課金）</li>
						<li>CMSサービスの利用料（月額費用）</li>
						<li>決済サービスの利用料（決済ごとの手数料）</li>
					</ul>
				</dd>
				<dt>仕様</dt>
				<dd>
					<ul>
						<li>オリジナルデザイン</li>
						<li>固定ページA4サイズ5ページまで</li>
						<li>独自ドメイン</li>
						<li>サーバーレス</li>
						<li>ヘッドレスCMS</li>
						<li>オンライン決済</li>
					</ul>
				</dd>
			</dl>
			<div class="stripe">
				<div class="catalog">
					<img src={plan_EC} alt="plan" width="288" height="288" />
					<script async src="https://js.stripe.com/v3/buy-button.js">
					</script>

					<stripe-buy-button
						buy-button-id="buy_btn_1O6va2AIPjnW5yZ1N3wRK47m"
						publishable-key="pk_live_51O4Nt8AIPjnW5yZ1xpcThU3EhrRdaLkVHN9YDM0otNAgKHrVoUwdLyZD7BHzJ1FvsFm7QoG2L2nn8kpEz2bsKLV000CU0ShlND"
					/>
				</div>
			</div>
		</div>
	</section>
</main>

<style>
	.contentsTop {
		border-top: solid 2px black;
		border-bottom: solid 2px black;
		padding-bottom: 1rem;
	}
	ol {
		width: fit-content;
		margin: auto;
	}
	.data {
		display: grid;
		grid-template-columns: 80px auto;
	}
	.data dt:nth-of-type(4) {
		border-bottom: solid 2px black;
	}
	.data dd:nth-of-type(4) {
		border-bottom: solid 2px black;
	}
	.data dd:nth-of-type(2) {
		font-size: 2rem;
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
	.catalog {
		position: relative;
	}
	stripe-buy-button {
		display: grid;
		line-height: 1rem;
		position: absolute;
		bottom: 0;
	}
	@media (width <= 800px) {
		.plan {
			display: initial;
		}
		.stripe {
			margin: 8px auto;
		}
	}
	@media (width >= 1200px) {
		.TopContents .image img {
			max-height: 300px;
		}
	}
</style>
