<template>
    <div class="software_section">
        <div>
            <h1 class="font-dm-sans font-bold custom_fjeRt">
                Aren’t these software outsourcing challenges familiar?
            </h1>
        </div>
        <div>
            <div>
                    <h2 class="font-dm-sans">Local talent storage</h2>
                    <p>You have to compete with tech giants to hire developers near you</p>
            </div>
            <div>
                    <h2 class="font-dm-sans">Lack of flexibity</h2>
                    <p>Scaling your team up & down causes unbearable admin hassle</p>
            </div>
            <div>
                    <h2 class="font-dm-sans">Slow hiring</h2>
                    <p>Acquiring senior programmers and QA engineers takes forever</p>
            </div>
            <div>
                    <h2 class="font-dm-sans">Clash of cultures</h2>
                    <p>You struggle to integrate remote offshore developers into your team</p>
            </div>
        </div>
    </div>
</template>
<style lang="scss">
.software_section {
    background: var(--var-color-prim);
    color: var(--var-color-sec);
    padding: 8vh 5%;
    margin-top: 20vh;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: center;
    flex-wrap: wrap-reverse;

    .custom_fjeRt {
        font-size: calc(10px + 3.6vmin);
    }
    div {
        vertical-align: top;
        margin: 20px;


        &:nth-child(2) {
            display: flex;
            flex-direction: row;
            align-items: center;
            flex-wrap: wrap;
            height: max-content;
            margin-bottom: 40px;

            div {
                width: 350px;
                height: 240px;
                display: flex;
                transition: all 0.3s ease-out;
                flex-direction: column;
                align-items: flex-start;
                justify-content: center;
                margin: 6px;
                background: var(--var-color-sec);
                padding: 20px;
                border-radius: 7px;
                color: var(--var-color-prim);


                p {
                    font-family: 'Plus Jakarta Sans', sans-serif;
                    margin-top: 6px;
                }

                h2 {
                    font-size: calc(10px + 2vmin);
                }
            }
        }
    }
}

</style>