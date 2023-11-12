<script lang="ts" context="module">
	import DataTable from './data-table.svelte';

	export type Payment = {
		id: string;
		amount: number;
		status: 'pending' | 'processing' | 'success' | 'failed';
		email: string;
	};

	const payments: Payment[] = [
		{
			id: 'abc123',
			amount: 50.75,
			status: 'pending',
			email: 'john.doe@example.com',
		},
		{
			id: 'xyz456',
			amount: 120.0,
			status: 'processing',
			email: 'jane.smith@example.com',
		},
		{
			id: '123def',
			amount: 85.25,
			status: 'success',
			email: 'bob.jones@example.com',
		},
		{
			id: '789ghi',
			amount: 30.5,
			status: 'failed',
			email: 'alice.davis@example.com',
		},
		{
			id: 'qwe789',
			amount: 65.2,
			status: 'pending',
			email: 'sam.wilson@example.com',
		},
		{
			id: 'rty456',
			amount: 150.5,
			status: 'processing',
			email: 'lisa.anderson@example.com',
		},
		{
			id: 'uio321',
			amount: 42.75,
			status: 'success',
			email: 'michael.jackson@example.com',
		},
		{
			id: 'zxc987',
			amount: 75.8,
			status: 'failed',
			email: 'susan.miller@example.com',
		},
		{
			id: 'vbn654',
			amount: 90.25,
			status: 'pending',
			email: 'kevin.white@example.com',
		},
		{
			id: 'mnb321',
			amount: 110.0,
			status: 'processing',
			email: 'emily.jones@example.com',
		},
		{
			id: 'lkj987',
			amount: 20.5,
			status: 'success',
			email: 'david.thompson@example.com',
		},
		{
			id: 'poi456',
			amount: 55.75,
			status: 'failed',
			email: 'olivia.smith@example.com',
		},
		{
			id: 'zxc123',
			amount: 80.4,
			status: 'pending',
			email: 'alex.walker@example.com',
		},
		{
			id: 'vbn789',
			amount: 95.6,
			status: 'processing',
			email: 'grace.roberts@example.com',
		},
	];
</script>

<div class="flex justify-center content-center">
	<DataTable data={payments} />
</div>
