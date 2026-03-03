<template>
    <div class="flex flex-col justify-center">
        <div>
            <TitleCard className="flex items-center flex-col gap-5 pb-10 dark:text-primary/80">
                Soutenez mon travail
            </TitleCard>
        </div>
    
        <div class="p-6 flex flex-col items-center z-1">
            <p class="text-mutedForeground pt-6 text-lg desktop:w-210">Cette section est temporairement indisponible. <br>
            Pour tout soutien financier, vous pouvez effectuer votre versement via le numéro indiqué ci-dessous (mobile monay). <br>
            Pour toute information complémentaire ou assistance, ce même numéro reste à votre disposition.<br><a class="no-underline hover:underline text-blue-600" href="tel:+243821600256">+243 821 600 256</a>
            </p>
        </div>

            <div class="tablette:flex desktop:justify-center flex-col desktop:flex-row flex justify-center">
                <Layoutprimary autherClass="flex flex-col items-center tablette:w-55 transition duration-700 hover:-translate-y-1 ease-in-out hover:shadow-[0px_10px_93px_-73px_#4D9FA3]">
                    <Like/>
                </Layoutprimary>
                <Layoutprimary autherClass="flex flex-col items-center tablette:w-55 transition duration-700 hover:-translate-y-1 ease-in-out hover:shadow-[0px_10px_93px_-73px_#4D9FA3]">
                    <DIscussion/>
                </Layoutprimary>
                <Layoutprimary autherClass="flex flex-col items-center tablette:w-55 transition duration-700 hover:-translate-y-1 ease-in-out hover:shadow-[0px_10px_93px_-73px_#4D9FA3]">
                    <Finacement/>
                </Layoutprimary>
        </div>
        <!-- <div class="flex justify-center">
            <div class="desktop:w-210">
                <Layoutprimary autherClass="flex flex-col items-center">
                    <FinanceSecondary/>
                </Layoutprimary>
            </div>
        </div> -->
    </div>
</template>

<script setup>
import TitleCard from '../TitleCard.vue';
import Layoutprimary from '../Layoutprimary.vue';
import Like from './Like.vue';
import DIscussion from './DIscussion.vue';
import Finacement from './Finacement.vue';
// import FinanceSecondary from './FinanceSecondary.vue';
</script>