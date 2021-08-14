<script context='module'>
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>Pricing</title>
</svelte:head>

<div class='pricing-header p-3 pb-md-4 mx-auto text-center'>
	<h1 class='display-4 fw-normal'>Pricing</h1>
	<p class='fs-5 text-muted'>Quickly build an effective pricing table for your potential customers with this Bootstrap
		example. It’s built with default Bootstrap components and utilities with little customization.</p>
</div>


<div class='row row-cols-1 row-cols-md-3 mb-3 text-center'>
	<div class='col'>
		<div class='card mb-4 rounded-3 shadow-sm'>
			<div class='card-header py-3'>
				<h4 class='my-0 fw-normal'>Free</h4>
			</div>
			<div class='card-body'>
				<h1 class='card-title pricing-card-title'>$0<small class='text-muted fw-light'>/mo</small></h1>
				<ul class='list-unstyled mt-3 mb-4'>
					<li>10 users included</li>
					<li>2 GB of storage</li>
					<li>Email support</li>
					<li>Help center access</li>
				</ul>
				<button class='w-100 btn btn-lg btn-outline-primary' type='button'>Sign up for free</button>
			</div>
		</div>
	</div>
	<div class='col'>
		<div class='card mb-4 rounded-3 shadow-sm'>
			<div class='card-header py-3'>
				<h4 class='my-0 fw-normal'>Pro</h4>
			</div>
			<div class='card-body'>
				<h1 class='card-title pricing-card-title'>$15<small class='text-muted fw-light'>/mo</small></h1>
				<ul class='list-unstyled mt-3 mb-4'>
					<li>20 users included</li>
					<li>10 GB of storage</li>
					<li>Priority email support</li>
					<li>Help center access</li>
				</ul>
				<button class='w-100 btn btn-lg btn-primary' type='button'>Get started</button>
			</div>
		</div>
	</div>
	<div class='col'>
		<div class='card mb-4 rounded-3 shadow-sm border-primary'>
			<div class='card-header py-3 text-white bg-primary border-primary'>
				<h4 class='my-0 fw-normal'>Enterprise</h4>
			</div>
			<div class='card-body'>
				<h1 class='card-title pricing-card-title'>$29<small class='text-muted fw-light'>/mo</small></h1>
				<ul class='list-unstyled mt-3 mb-4'>
					<li>30 users included</li>
					<li>15 GB of storage</li>
					<li>Phone and email support</li>
					<li>Help center access</li>
				</ul>
				<button class='w-100 btn btn-lg btn-primary' type='button'>Contact us</button>
			</div>
		</div>
	</div>
</div>

<h2 class='display-6 text-center mb-4'>Compare plans</h2>

<div class='table-responsive'>
	<table class='table text-center'>
		<thead>
		<tr>
			<th style='width: 34%;'></th>
			<th style='width: 22%;'>Free</th>
			<th style='width: 22%;'>Pro</th>
			<th style='width: 22%;'>Enterprise</th>
		</tr>
		</thead>
		<tbody>
		<tr>
			<th class='text-start' scope='row'>Public</th>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
		</tr>
		<tr>
			<th class='text-start' scope='row'>Private</th>
			<td></td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
		</tr>
		</tbody>

		<tbody>
		<tr>
			<th class='text-start' scope='row'>Permissions</th>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
		</tr>
		<tr>
			<th class='text-start' scope='row'>Sharing</th>
			<td></td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
		</tr>
		<tr>
			<th class='text-start' scope='row'>Unlimited members</th>
			<td></td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
		</tr>
		<tr>
			<th class='text-start' scope='row'>Extra security</th>
			<td></td>
			<td></td>
			<td>
				<svg class='bi' height='24' width='24'>
					<use xlink:href='#check' />
				</svg>
			</td>
		</tr>
		</tbody>
	</table>
</div>

<style>
    .pricing-header {
        max-width: 700px;
    }
</style>
