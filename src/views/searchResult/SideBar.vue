<template>
    <ul class="list-group  list-sidebar-style mb-30 box-shadow">
        <li class="list-group-item">
            <h6 class="font-weight-600">ค้นหาบ้านของคุณ</h6>
            <div class="search_area">
                <input type="text" class="form-control form-control-text " placeholder="คุณกำลังมองหาอะไรอยู่"><span>
                <i class="fa-solid fa-magnifying-glass"></i></span>
            </div>
        </li>

        <li class="list-group-item">
            <h6 class="font-weight-600">สถานะการขาย</h6>
            <div class="radio-element">

                <div class="form-check">
                    <input class="form-check-input radio-style" type="radio" name="exampleRadios" id="exampleRadios1" value="option1"
                        checked>
                    <label class="form-check-label font-style" for="exampleRadios1">ทั้งหมด</label>
                </div>
                <div class="form-check">
                    <input class="form-check-input radio-style" type="radio" name="exampleRadios" id="exampleRadios2" value="option2">
                    <label class="form-check-label font-style" for="exampleRadios2">ซื้อ</label>
                </div>
                <div class="form-check ">
                    <input class="form-check-input radio-style" type="radio" name="exampleRadios" id="exampleRadios3" value="option3">
                    <label class="form-check-label font-style" for="exampleRadios3">เช่า</label>
                </div>
            </div>
        </li>

        <li class="list-group-item">
            <h6 class="font-weight-600">ประเภทอสังหาริมทรัพย์</h6>

            <div class="form-check  custom-checkbox">
                <input class="form-check-input  checkboox-all custom-control-input " type="checkbox" value="" id="All"  onclick="selectAll()">
                <label class="form-check-label custom-control-label font-style" for="All">ทั้งหมด</label>
            </div>
            <div class="form-check custom-checkbox">
                <input class="form-check-input  checkboox-all custom-control-input " type="checkbox" value="" id="Houses" onclick="checkAll()">
                <label class="form-check-label custom-control-label font-style" for="Houses">บ้าน</label>
            </div>
            <div class="form-check custom-checkbox">
                <input class="form-check-input checkboox-all custom-control-input " type="checkbox" value="" id="Apartments" onclick="checkAll()">
                <label class="form-check-label custom-control-label font-style" for="Apartments">อพาร์ตเมนต์</label>
            </div>
            <div class="form-check  custom-checkbox">
                <input class="form-check-input checkboox-all custom-control-input " type="checkbox" value="" id="Office" onclick="checkAll()">
                <label class="form-check-label custom-control-label font-style" for="Office">สำนักงาน</label>
            </div>
            <div class="form-check custom-checkbox">
                <input class="form-check-input checkboox-all custom-control-input " type="checkbox" value="" id="Villa" onclick="checkAll()">
                <label class="form-check-label custom-control-label font-style" for="Villa">วิลล่า</label>
            </div>

        </li>
        <li class="list-group-item">
            <h6 class="font-weight-600">ช่วงราคา</h6>

              <div class="row">
                <div class="col-12">
                    <div class="form-check  custom-checkbox">
                        <input class="form-check-input custom-control-input checkboox-price " type="checkbox" value="" id="averageAll" onclick="priceAll()" >
                        <label class="form-check-label custom-control-label font-style" for="averageAll">ทั้งหมด</label>
                    </div>
                </div>
                <div class="col-lg-12">
                    <div class="form-check  custom-checkbox">
                        <input class="form-check-input custom-control-input checkboox-price" type="checkbox" value="" id="1Million" onclick="checkPrice()" >
                        <label class="form-check-label custom-control-label font-style" for="1Million">
                            ฿1,000,000
                        </label>
                    </div>
                </div>
                <div class="col-lg-12">
                    <div class="form-check  custom-checkbox">
                        <input class="form-check-input custom-control-input checkboox-price" type="checkbox" value="" id="5Million"  onclick="checkPrice()" >
                        <label class="form-check-label custom-control-label font-style" for="5Million">
                            ฿1,000,001 - ฿5,000,000
                        </label>
                    </div>
                </div>
                <div class="col-lg-12">
                    <div class="form-check  custom-checkbox">
                        <input class="form-check-input custom-control-input checkboox-price" type="checkbox" value="" id="10Million"  onclick="checkPrice()" >
                        <label class="form-check-label custom-control-label font-style" for="10Million">
                            ฿5,000,000 - ฿10,000,000
                        </label>
                    </div>
                </div>
                <div class="col-lg-12">
                    <div class="form-check  custom-checkbox">
                        <input class="form-check-input custom-control-input checkboox-price" type="checkbox" value="" id="10MillionUp"  onclick="checkPrice()" >
                        <label class="form-check-label custom-control-label font-style" for="10MillionUp">
                            ฿10,000,001
                        </label>
                    </div>
                </div>
              </div>
        </li>
        <li class="list-group-item">
              <div class="form-group">
                <h6 class="font-weight-600">ที่ตั้ง</h6>
                <select class="form-control" id="exampleFormControlSelect1">
                    <option>กรุงเทพ</option>
                    <option>ปทุมธานี</option>
                    <option>นนทบุรี</option>
                    <option>อยุธยา</option>
                </select>
              </div>
        </li>

        <li class="list-group-item">
            <h6 class="font-weight-600">ห้องนอน</h6>
            <div class="d-flex justify-content-center">
                <div class="selection">
                    <input type="radio" id="any" name="Bedrooms" checked>
                    <label for="any">ทั้งหมด</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus1" name="Bedrooms">
                    <label for="plus1">+1</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus2" name="Bedrooms">
                    <label for="plus2">+2</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus3" name="Bedrooms">
                    <label for="plus3">+3</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus4" name="Bedrooms">
                    <label for="plus4">+4</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus5" name="Bedrooms">
                    <label for="plus5">+5</label>
                </div>
            </div>
        </li>

        <li class="list-group-item">
            <h6 class="font-weight-600">ห้องน้ำ</h6>
            <div class="d-flex justify-content-center">
                <div class="selection">
                    <input type="radio" id="anyBathrooms" name="Bathrooms" checked>
                    <label for="anyBathrooms">ทั้งหมด</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus1Bathrooms" name="Bathrooms">
                    <label for="plus1Bathrooms">+1</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus2Bathrooms" name="Bathrooms">
                    <label for="plus2Bathrooms">+2</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus3Bathrooms" name="Bathrooms">
                    <label for="plus3Bathrooms">+3</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus4Bathrooms" name="Bathrooms">
                    <label for="plus4Bathrooms">+4</label>
                </div>
                <div class="selection">
                    <input type="radio" id="plus5Bathrooms" name="Bathrooms">
                    <label for="plus5Bathrooms">+5</label>
                </div>
            </div>
        </li>

        <li class="list-group-item">

            <button type="submit"
            class="btn btn-primary afterButton rounded-pill w-100 "
            id="submitModal">
            <i class="fa-solid fa-magnifying-glass"></i> ค้นหา
            </button>

        </li>
        <li class="list-group-item">
            <div class="d-flex justify-content-between">

                <a href="javascript:void(0)">
                    <span class="fa fa-repeat"></span>
                    <u>รีเซ็ตตัวกรองทั้งหมด</u>
                </a>
                <a href="javascript:void(0)">
                    <span class="fa fa-star"></span>
                    <u>บันทึกการค้นหา</u>
                </a>

            </div>
        </li>

    </ul>
</template>

<script>
export default {
    name:'SideBarVue',
    data(){
        return{

        }
    }

}
</script>

<style>
/* ---------------------------- ส่วน ปุ่มค้นหา ------------------------------------------ */

.search_area {
    position: relative;
}

.search_area .form-control-text {
    padding-left: 42px;
}

.search_area span {
    font-size: 18px;
    left: 12px;
    position: absolute;
    top: 5px;
}



/* ---------------------------- ส่วน checkbox ------------------------------------------ */

.custom-checkbox .custom-control-input:checked ~ .custom-control-label::before {
    background-color: #0071bc;
}

/* ---------------------------- ส่วน radio ------------------------------------------ */

.price-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0 10px;
}

.radio-style {
    /* bottom: 4px;
    height: 20px;
    width: 20px; */
    accent-color: #0071bc;
  }

/* ---------------------------- ส่วน Bedrooms ------------------------------------------ */

.selection:first-child label {
    border-radius: 12px 0 0 12px;
}

.selection:last-child label {
    border-radius: 0 12px 12px 0;
}

.selection label {
    background-color: #fff;
    border: 2px solid transparent;
    cursor: pointer;
    display: inline-block;
    color: #080808;
    font-weight: 600;
    font-size: 13px;
    outline: 1px solid #dddddd;
    margin-right: 1px;
    padding: 7px 12px;
}

.selection input[type="radio"] {
    display: none;
}

.selection input[type="radio"]:checked ~ label {
    border: 2px solid #0071bc !important;
    /* outlinie: transparent; */
    z-index: 1;
}
</style>