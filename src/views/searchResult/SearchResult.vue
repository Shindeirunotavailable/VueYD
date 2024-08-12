<template>
    <section class="background-grey pt-30 pb-30">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <h2>บ้านเพื่อขาย</h2>
                </div>
            </div>
        </div>
    </section>

    <section>
        <div class="container">
            <div class="mobile-laptop">
                <div class="row mb-15">
                    <div class="col-12 col-lg-12">
                        <div class="d-flex justify-content-end">
                            <div class="pcs_dropdown">
                                <label class="mr-10">เรียงตาม</label>
                                <select class="form-select">
                                    <option>ขายดี</option>
                                    <option>การจับคู่ที่ดีที่สุด</option>
                                    <option>ราคาต่ำ</option>
                                    <option>ราคาสูง</option>
                                </select>
                            </div>
                            <label class="ml-10 border-right"></label>

                            <div class="nav" id="nav-tab" role="tablist">
                                <div class="ml-10 mr-10 link-effect active" id="nav-profile-tab" data-toggle="tab"
                                    data-target="#nav-profile" type="button" role="tab" aria-controls="nav-profile"
                                    aria-selected="true">
                                    <p>กริด</p>
                                </div>
                                <label class="border-right"></label>
                                <div class="ml-10 link-effect" id="nav-contact-tab" data-toggle="tab"
                                    data-target="#nav-contact" type="button" role="tab" aria-controls="nav-contact"
                                    aria-selected="false">
                                    <p>รายการ</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="tab-content row" id="nav-tabContent">
                    <div class="col-lg-4">
                        <SideBarVue />
                    </div>
                    <div class="tab-pane fade col-lg-8 show active" id="nav-profile" role="tabpanel"
                        aria-labelledby="nav-profile-tab">
                        <ListVue />
                    </div>
                    <div class="tab-pane fade col-lg-8" id="nav-contact" role="tabpanel"
                        aria-labelledby="nav-contact-tab">
                        <ListVue />
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import ListVue from './List.vue'
import SideBarVue from './SideBar.vue'

export default {
    name: 'SearchResultVue',
    components: {
        SideBarVue,
        ListVue,
    },
}
</script>

<style scoped>
/* ---------------------------- ส่วน gird-list box  ------------------------------------------ */

.list-sidebar-style1 {
    padding-top: 10px;
    background-color: #ffffff;
    border-radius: 12px;
}
.list-sidebar-style{
    border-radius: 12px;
}
.text-block {
    /* height: 35px; */
    border-radius: 10px;
    margin-left: 10px;
    position: absolute;
    margin-top: 195px;
    background-color: white;
    color: black;
    width: 115px;
    z-index: 1;
}

.text-list {
    /* height: 35px; */
    border-radius: 10px;
    margin-left: 10px;
    position: absolute;
    margin-top: 160px;
    background-color: white;
    color: black;
    width: 70px;
    z-index: 1;

}

.block-text {
    /* height: 30px; */
    border-radius: 10px;
    margin-left: 10px;
    position: absolute;
    margin-top: 10px;
    background-color: #0071bc;
    color: white;
    width: 90px;
    z-index: 1;
}

.block-list {
    height: 35px;
    border-radius: 10px;
    margin-left: 25px;
    position: absolute;
    margin-top: 10px;
    background-color: #0071bc;
    color: rgb(255, 255, 255);
    width: 100px;
}

.font-label {
    font-size: 13px;
}

.img-block {
    overflow: hidden;
}

.img-sell {
    position: relative;
    height: 230px;
}

.img-sell:hover {
    transition: transform 0.4s ease;
    transform: scale(1.1) rotate(-1deg);
}

.img-list{
  position: relative;
  height: 200px;
}

.img-list:hover {
  transition: transform 0.4s ease;
  transform: scale(1.1) rotate(-1deg);
}

/* .block-text:hover{
    transition: transform 0.4s ease, opacity 0.4s ease;
    transform: translateY(100%);
    opacity: 0;
  } */
   
.text-whiter{
    color: white;
}
.font-style {
    /* margin-left: 10px; */
    font-size: 13px;
    font-weight: 500;
}

.h-250 {
    height: 250px;
}
.h-60 {
    height: 60px;
}

.p-10 {
    padding: 10px;
}

.mr-165 {
    margin-right: 165px;
}


.font-weight-700{
    font-weight: 700;
}

.font-weight-500{
    font-weight: 500;
}

.font-weight-600{
    font-weight: 600;
}

.red:hover{
    color: red;
}

.blue:hover{
    color: #0071bc;
}

.green:hover{
    color: green;
}

.background-white{
    background-color: white;
}

.box-shadow{
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);

}

.box-shadow-lightblue{
    box-shadow: 5px 5px 5px rgba(41, 41, 41, 0.226);

}

.pb-auto{
    padding-bottom: auto;
}

.pt-auto{
padding-top: auto;
}

.font-size-13{
    font-size: 13px;
}

.p-15{
    padding: 15px   ;
}


.p-18{
    padding: 18px   ;
}

.color-yuudee{
    background-color: #0071bc !important;
}

</style>