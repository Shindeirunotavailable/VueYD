<template>
    <div class="container mt-4">
        <div class="row d-flex justify-content-center">
            <div class="col-md-9">
                <div class="p-4 mt-3">
                    <h3 class="heading mt-5 text-center">Hi! How can we help You?</h3>
                    <div class="d-flex justify-content-center px-5">
                        <div class="search">
                            <input type="text" class="search-input" placeholder="Search..." name="">
                            <button type="button" class="list-icon ml-10" data-toggle="modal" data-target="#exampleModal">
                                <i class="fa fa-list-ul"></i>  </button>
                            <a href="#" class="search-icon"> <i class="fa fa-search"></i> </a>
                        </div>
                    </div>
                    <div class="row mt-4 g-1 px-4 mb-5">
                        <div class="col-md-2">
                            <div class="card-inner p-3 d-flex flex-column align-items-center"> <img
                                    src="https://i.imgur.com/Mb8kaPV.png" width="50">
                                <div class="text-center mg-text"> <span class="mg-text">Account</span> </div>
                            </div>
                        </div>
                        <div class="col-md-2">
                            <div class="card-inner p-3 d-flex flex-column align-items-center"> <img
                                    src="https://i.imgur.com/ueLEPGq.png" width="50">
                                <div class="text-center mg-text"> <span class="mg-text">Payments</span> </div>
                            </div>
                        </div>
                        <div class="col-md-2">
                            <div class="card-inner p-3 d-flex flex-column align-items-center"> <img
                                    src="https://i.imgur.com/tmqv0Eq.png" width="50">
                                <div class="text-center mg-text"> <span class="mg-text">Delivery</span> </div>
                            </div>
                        </div>
                        <div class="col-md-2">
                            <div class="card-inner p-3 d-flex flex-column align-items-center"> <img
                                    src="https://i.imgur.com/D0Sm15i.png" width="50">
                                <div class="text-center mg-text"> <span class="mg-text">Product</span> </div>
                            </div>
                        </div>
                        <div class="col-md-2">
                            <div class="card-inner p-3 d-flex flex-column align-items-center"> <img
                                    src="https://i.imgur.com/Z7BJ8Po.png" width="50">
                                <div class="text-center mg-text"> <span class="mg-text">Return</span> </div>
                            </div>
                        </div>
                        <div class="col-md-2">
                            <div class="card-inner p-3 d-flex flex-column align-items-center"> <img
                                    src="https://i.imgur.com/YLsQrn3.png" width="50">
                                <div class="text-center mg-text"> <span class="mg-text">Guarantee</span> </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal -->
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="exampleModalLabel">More Filter</h5>
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">&times;</span>
                    </button>
                </div>
                <div class="modal-body">
                    







                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
                    <button type="button" class="btn btn-primary"> <i class="fa fa-search"></i> Search</button>
                </div>
            </div>
        </div>
    </div>


</template>

<script>
export default {
    name: 'Searchvue',
    data() {
        return {

        }
    }

}
</script>

<style scoped>
.ml-10 {
    margin-left: 10px;
}

.card {

    border: none;
    background: #eee;

}

.search {
    width: 100%;
    margin-bottom: auto;
    margin-top: 20px;
    height: 50px;
    background-color: #fff;
    padding: 10px;
    border-radius: 5px;
}

.search-input {
    color: white;
    border: 0;
    outline: 0;
    background: none;
    width: 0;
    margin-top: 5px;
    caret-color: transparent;
    line-height: 20px;
    transition: width 0.4s linear
}

.search .search-input {
    padding: 0 10px;
    width: 100%;
    caret-color: #536bf6;
    font-size: 19px;
    font-weight: 300;
    color: black;
    transition: width 0.4s linear;
}


.search-icon {
    height: 34px;
    width: 34px;
    float: right;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    background-color: #536bf6;
    font-size: 10px;
    bottom: 30px;
    position: relative;
    border-radius: 5px;
}

.list-icon {
    height: 34px;
    width: 34px;
    float: right;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    background-color: #3583eb;
    font-size: 10px;
    bottom: 30px;
    position: relative;
    border-radius: 5px;
}

.search-icon:hover {

    color: #fff !important;
}

a:link {
    text-decoration: none
}

.card-inner {
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-color: #fff;
    background-clip: border-box;
    border: 1px solid rgba(0, 0, 0, .125);
    border-radius: .25rem;
    border: none;
    cursor: pointer;
    transition: all 2s;
}


.card-inner:hover {

    transform: scale(1.1);

}

.mg-text span {

    font-size: 12px;

}

.mg-text {

    line-height: 14px;
}
</style>