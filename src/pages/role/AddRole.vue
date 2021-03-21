<template>
	<div class="p-grid">
		<div class="p-col-12 p-md-6">
			<div class="card p-fluid">
				<h4>Add Role</h4>
					<div class="p-field p-col">
						<label for="userId">Role ID</label>
						<InputText id="userId" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="role">Name</label>
						<InputText id="role" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col" id="activeState">
						<label for="active" id="activeToggle">Active</label>
                        <InputSwitch v-model="isActive" />
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
			return {
                isActive: false
            }
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

    #activeState {
        display: grid;
    }

    #activeToggle {
        margin: 0 0 10px 0;
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