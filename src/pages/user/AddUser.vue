<template>
	<div class="p-grid">
		<div class="p-col-12 p-md-6">
			<div class="card p-fluid">
				<h4>Add User</h4>
					<div class="p-field p-col">
						<label for="userId">User ID</label>
						<InputText id="userId" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="username">Username</label>
						<InputText id="username" type="text" placeholder="Type here..." />
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
						<label for="role">Role</label>
						<InputText id="role" type="text" placeholder="Type here..." />
					</div>
					<div class="p-field p-col">
						<label for="email2">Email</label>
						<InputText id="email2" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="name2">Name</label>
						<InputText id="name2" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="mobileNo">Mobile No</label>
						<InputText id="mobileNo" type="number" placeholder="Type here..." />
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