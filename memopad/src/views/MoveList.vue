<template>
    <h2>MoveList</h2>
    <div id = "container">
            <div id ="left-container">
                <div id="left-box">
                    <p>Apple</p>
                    <p>Grape</p>
                    <p>Strawberry</p>
                    <p>Cherry</p>
                    <p>Plum</p>
                </div>
                <button id="left-btn">右へ移動</button>
            </div>
            <div id = "right-container">
                <div id="right-box">
                    <p>Watermelon</p>
                    <p>Banana</p>
                    <p>Peach</p>
                </div>
                <button id="right-btn">左へ移動</button>
            </div>
        </div>
</template>

<style>
#container {
    width: 700px;
    margin: 50px auto;
    display: flex;
    justify-content: space-between;
}
#left-container,#right-container {
    width: 300px;
    height: 500px;
}
#left-box,#right-box {
        width: 100%;
        height: 100%;
        border: 1px solid navy;
        display: inline-block;
        text-align: center;
    }

#right-btn,#left-btn {
        background-color: navy;
        color: white;
        margin: 30px auto;
        height: 40px;
        width: 150px;
        font-size: 16px;
        cursor: pointer;
        display: block;
        border: none;
    }
p {
    width: 80%;
    border-bottom: solid 1px navy;
    margin: 0 auto;
    line-height: 50px;
    display: block;
}
</style>