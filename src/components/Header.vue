<template>
    <div class="header">
        <div class="item">
            <p>Menu 1</p> 
            <span class="menu1">
                <ul>Some menu item 1</ul>
                <ul>Some menu item 1</ul>
                <ul>Some menu item 1</ul>
                <ul>Some menu item 1</ul>
            </span>        
        </div>
        <div class="item">
            <p>Menu 2</p>
            <span class="menu2">
                <ul>Some menu item 2</ul>
                <ul>Some menu item 2</ul>
                <ul>Some menu item 2</ul>
                <ul>Some menu item 2</ul>
            </span>        
        </div>
    </div>
</template>
<script>
export default {
    name:'Header'
}
</script>
<style >
.header{
    background: #efefef;
    width: 100%;
    border-radius: 10px;
    height: 56px;
    position: relative;
    z-index: 1;
}
.header .item{
    display: inline-block;
    height: 56px;
    padding: 0px 5px;
}
.item p{
    line-height: 56px;
    background:transparent;
    margin: 0px;

}
 p:hover + span{
    display: block;
}

.item span{
    display: none;
    background: #e3e3e3;
    position: absolute;
    margin-top:10px; 
    width: 100%;
    left: 0;
    border-radius: 10px;
}
ul{
    padding: 0px;
    margin-left: 10px;
}

</style>
