<script>
    
	import HomeHeroSec1 from '../components/HomeHeroSec1.svelte';
	import Timeline from '../components/Timeline.svelte';

    export let timelineData = [{
        title: "Fast T-Shirt Print",
        imgsrc: "./Embroidered-Branded-Workwear-For-Financial-Services.jpg",
        left: true,
        desc: `From one-off to bulk orders, we offer same day and next day t-shirt printing. Serving all of London and the United Kingdom. International orders also available.
        Our QUICK GET A QUOTE FORM is fast, simple and easy. Just tell us what you need, how many items you need, and we will give you an answer as fast as possible.`
    },
    {
        title: "Urgent Orders",
        imgsrc: "./Printed-Running-Shirts-for-New-Forest-Marathon.jpg",
        left: false,
        desc: `If you have an order that requires urgency we have the resources and the expertise to meet your needs quickly and effectively. Whether you require printed polo shirts for a corporate sponsorship, need custom t-shirts for a charity event, or specialised printed sportswear, we can help you!`
    },
    {
        title: "No Minimum Order",
        imgsrc: "./personalised-caps-for-partnership.jpg",
        left: true,
        desc: `We have built a one-of-a-kind reputation for providing LAST MINUTE FAST T-SHIRT PRINTING with same day orders and next day EXPRESS delivery. Our fast turnaround and competitive prices are what set us apart from our competitors. We use the latest in industry technology to offer our customers the highest quality services and at the fastest possible turnaround.`
    }];
</script>



<HomeHeroSec1 />
<div
  class="lg:px-16 px-6 py-8 text-center"
>

    <h1 class="text-4xl font-bold my-2 py-2 italic text-shades-900">Fast T-Shirt Printing and Express Delivery</h1>
    <h4 class="mb-16 leading-relaxed text-xl font-normal">Customise your own t-shirts, hoodies and other personalised clothing garments and get them done same day with next day express delivery available.</h4>
 
{#each timelineData as item}
    <Timeline title={item.title} imgsrc={item.imgsrc} left={item.left} desc={item.desc}/>
{/each}
</div>