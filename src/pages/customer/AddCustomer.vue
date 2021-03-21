<template>
	<div class="p-grid">
		<div class="p-col-12 p-md-6">
			<div class="card p-fluid">
				<h4>Add Customer</h4>
					<div class="p-field p-col">
						<label for="customerId">Customer ID</label>
						<InputText id="customerId" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="firstName">First Name</label>
						<InputText id="firstName" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="lastName">Last Name</label>
						<InputText id="lastName" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="telephoneNo">Telephone No</label>
						<InputText id="telephoneNo" type="number" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="mobileNo">Mobile No</label>
						<InputText id="mobileNo" type="number" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="address">Address</label>
						<InputText id="address" type="text" placeholder="Type here..." />
					</div>
					<div class="p-field p-col">
						<label for="email2">Email</label>
						<InputText id="email2" type="text" placeholder="Type here..." />
					</div>
			</div>
		</div>
    </div>
    <div class="p-col-12 p-md-6" id="saveBtn">
        <Button label="Save" icon="pi pi-check" />
    </div>
</template>
<script>
	export default {
		data() {
			return {}
		}
	}
</script>
<style scoped>
    h4 {
        margin: 0 0 20px 8px;
    }

    #saveBtn {
        display: flex;
        justify-content: flex-end;
    }

    @media screen and (max-width: 1025px){
        .p-md-6 {
            width: 100%;
        }
    }

    @media screen and (max-height: 768px){
        .p-md-6 {
            width: 50%;
        }
    }
</style>