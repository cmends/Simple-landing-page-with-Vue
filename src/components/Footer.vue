<template>
    <footer>
        <div class="footer-top">
            <div class="footer-1">
                <span>Contact Us</span>
                <p>30 KpaKpaKpa Estate,Accra, <br>
                    Ghana.</p>
                <p>KpaKpaKpa.gh</p>
                <p>info@kpakpakpa.gh</p>
                <p>+233419419419</p>
            </div>
        </div>

       


        <div class="footer-bottom">


            <p>Copyright©2022 KpaKpaKpa
            </p>

            <p>
                Privacy & Policy
            </p>
        </div>
    </footer>

</template>

<script>
export default {
    name: "Appfooter"
};
</script>

<style scoped>
footer {
    width: 100%;
    left: 0;
    padding: 90px;
    color:black;
    background: rgb(221, 194, 43);
    /* bottom: 0; */
    /* position: absolute; */
}

footer p {
    color:black;
    font-weight: 400;
    font-size: 14px;
    line-height: 19px;
}

.footer-top {
    display: flex;
}

.footer-1 {
    margin-right: 550px;
}

.footer-1 span,
.footer-1 p {
    margin-bottom: 22px;
}

.footer-bottom {
    border-top: 3px solid;
    padding-top: 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>