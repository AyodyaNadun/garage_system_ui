<template>
	<div class="p-grid">
		<div class="p-col-12 p-md-6">
			<div class="card p-fluid">
				<h4>Add Vehicle</h4>
					<div class="p-field p-col">
						<label for="vehicleId">Vehicle ID</label>
						<InputText id="vehicleId" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="vehicleTypeId">Vehicle Type ID</label>
						<InputText id="vehicleTypeId" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="vin">VIN</label>
						<InputText id="vin" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="chassisNo">Chassis No</label>
						<InputText id="chassisNo" type="text" placeholder="Type here..." />
					</div>
                    <div class="p-field p-col">
						<label for="engineNo">Engine No</label>
						<InputText id="engineNo" type="text" placeholder="Type here..." />
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