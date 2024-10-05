<template>
    <div v-for="n in test" class="my_card col p-3 text-center">
        <a class="card_body border rounded-3 h-100 d-flex flex-column justify-content-around text-black">
            <div class="h-50 d-flex justify-content-center">
                <img class="img-fluid rounded-circle"
                    src="https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcSC4DtHTGprsp7K8u0ZlfSDmIDplvQYH5vniT0I3rpcl6wqBh8b"
                    alt="">
            </div>
            <div>{{ n }}</div>
        </a>
    </div>
    <div class="my_card col p-3 text-center">
        <div class="card_body border rounded-3 h-100 d-flex flex-column justify-content-around">
            <div class="h-50 d-flex justify-content-center">
                <div class="add_btn border rounded-circle d-flex justify-content-center align-items-center fs-1"></div>
            </div>
            <div>Add</div>

        </div>
    </div>
</template>

<style>
.my_card {
    height: 200px;
}

.my_card .card_body{
    text-decoration: none;
}

.my_card .card_body:hover{
    background-color: gray;
    transform: scale(1.1);
    transition: 0.3s ease;
}

.add_btn {
    height: 100%;
    max-width: 50%;
    aspect-ratio: 1 / 1;
    position: relative;
}

.add_btn::after {
    content: "";
    position: absolute;
    background-color: black;
    width: 50%;
    height: 0.5rem;
    border-radius: 10px;
}

.add_btn::before {
    content: "";
    position: absolute;
    background-color: black;
    width: 0.5rem;
    height: 50%;
    border-radius: 10px;
}
</style>

<script>
export default {
    data() {
        return {
            test: [1, 2, 3, 4, 5, 6]
        }
    }
}
</script>