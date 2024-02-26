<script>
  let sitetitle = "Richards Lodge 1116";
  // import { ModeWatcher } from "mode-watcher";
  import { Button } from "$lib/components/ui/button";
  import Sun from "lucide-svelte/icons/sun";
  import Moon from "lucide-svelte/icons/moon";
  import * as Card from "$lib/components/ui/card";
  import * as HoverCard from "$lib/components/ui/hover-card";
  import * as Table from "$lib/components/ui/table";
  import { toggleMode } from "mode-watcher";
</script>

<header class="py-5 container">
  <div id="header-inner" class="flex flex-col sm:flex-row gap-8 justify-between items-center mx-auto">
    <div id="site-title" class="text-center sm:text-left">
      <a href="/" class="flex flex-row items-center gap-4 justify-center sm:justify-start">
        <img class="max-w-14 inline-block" src="/RichardsLodge1116Logo.webp" alt="Richards Lodge 1116 Logo">
        <div >Richards Lodge 1116</div>
      </a>
    </div>
    <!-- <div class="text-sm sm:text-base text-center">April 6, 2024 at Yankee's Tavern in Carlos, Texas</div>
    <div id="main-nav" class="flex flex-col sm:flex-row items-center justify-end gap-4">
      <Button>Register</Button> 
      <div id="theme-toggle">
        <Button on:click={toggleMode} variant="outline" size="icon">
          <Sun class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0" />
          <Moon class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100" />
          <span class="sr-only">Toggle theme</span>
        </Button>
      </div>
    </div> -->
  </div>
</header>

<section class="my-20">
  <div class="container">
    <div class="flex flex-col lg:flex-row mg:items-center mx-auto lg:gap-20 gap-5">
      <div class="lg:max-w-[50%] mx-auto text-left">
        <h2 class="lg:text-xl my-2 tracking-wider">
          <span class="uppercase text-primary-foreground bg-primary px-4 py-2 rounded-md font-semibold leading-loose">16th Annual Richards Lodge 1116</span><br>
          <span class="text-6xl md:text-8xl leading-none font-bold">Car Show <br><span class="text-ring">&</span> Fundraiser</span>
        </h2>
        <p class="lg:text-xl lg:my-3">Join us at Yankee's Tavern in Carlos, Texas on April 6, 2024. Proceeds from this event go to support the local charities and communities in need that Richards Lodge is actively involved with.</p>
      </div>
      <div class="bg-[url('/CarShowGeneGallin.jpg')] bg-cover w-full lg:w-1/2 h-48 lg:h-96 bg-no-repeat bg-center">
        <!-- Image section remains the same -->
      </div>
    </div>
  </div>
</section>

<section class="my-24 container">
  <div class="max-w-[1000px] mx-auto">
    <p class="text-2xl lg:text-5xl text-center">Food • Music • Door Prizes</p>
    <p class="text-lg lg:text-4xl text-center mt-5 capitalize">Open to the public • Doors open at 8:00 AM</p>
    <p class="text-lg lg:text-4xl text-center mt-3 capitalize">Awards presentation is at 2:00 PM</p>
    <p class="lg:text-xl text-center my-5 max-w-[600px] mx-auto">
      25 awards for cars, trucks, jeeps, and bikes ⭐️ Children's pick ⭐️ Lodge Master pick ⭐️ Yankee Mike's pick ⭐️ Rat rod pick
    </p>
  </div>
</section>

<section class="mt-28 mb-20">
  <div class="max-w-6xl mx-auto px-4">
    <h2 class="text-3xl lg:text-4xl font-semibold text-center text-accent-foreground">Our Sponsors</h2>
    <div class="border-b-2 border-primary pt-4 mb-10 w-10 items-center mx-auto"></div>
    <div class="grid grid-cols-2 sm:grid-cols-5 gap-8 justify-center items-center">
      <!-- Sponsor Logos -->
      <!-- Repeat the structure below for each sponsor logo -->
      <div class="flex justify-center">
        <HoverCard.Root>
          <HoverCard.Trigger><img src="/logos/exlogo1.webp" alt="Sponsor 1" class="h-auto max-h-16"></HoverCard.Trigger>
          <HoverCard.Content>
            These are details about the sponsor. We love our sponsors.
          </HoverCard.Content>
        </HoverCard.Root>
      </div>
      <!-- Sponsor Logo 2 -->
      <div class="flex justify-center">
      <HoverCard.Root>
        <HoverCard.Trigger><img src="/logos/exlogo2webp.webp" alt="Sponsor 2" class="h-auto max-h-16"></HoverCard.Trigger>
        <HoverCard.Content>
          These are details about the sponsor. We love our sponsors.
        </HoverCard.Content>
      </HoverCard.Root>
    </div>
    <!-- Sponsor Logo 3 -->
    <div class="flex justify-center">
      <HoverCard.Root>
        <HoverCard.Trigger> <img src="/logos/exlogo3.webp" alt="Sponsor 3" class="h-auto max-h-16"></HoverCard.Trigger>
        <HoverCard.Content>
          These are details about the sponsor. We love our sponsors.
        </HoverCard.Content>
      </HoverCard.Root>
    </div>
    <!-- Sponsor Logo 4 -->
    <div class="flex justify-center">
      <HoverCard.Root>
        <HoverCard.Trigger> <img src="/logos/exlogo4.webp" alt="Sponsor 4" class="h-auto max-h-16"></HoverCard.Trigger>
        <HoverCard.Content>
          These are details about the sponsor. We love our sponsors.
        </HoverCard.Content>
      </HoverCard.Root>
    </div>
    <!-- Sponsor Logo 5 -->
    <div class="flex justify-center">
      <HoverCard.Root>
        <HoverCard.Trigger> <img src="/logos/exlogo5.webp" alt="Sponsor 4" class="h-auto max-h-16"></HoverCard.Trigger>
        <HoverCard.Content>
          These are details about the sponsor. We love our sponsors.
        </HoverCard.Content>
      </HoverCard.Root>
    </div>
  </div>
    </div>
  
</section>

<section class="container mb-28">
  <div class="max-w-[600px] mx-auto text-center my-10">
    <h2 class="text-2xl text-center font-semibold my-2">Sponsorship Opportunities</h2>
    <p>Our sponsors are so important... Lorem ipsum dolor sit amet, qui minim labore adipisicing... This how it works:</p>
  </div>
  <div class="overflow-x-auto">
    <div class="max-w-[800px] mx-auto">
      <div class="max-w-[500px] mx-auto">
          <Table.Root>
            <Table.Caption>For more information, contact: Scott Harman (936) 870-8505, Jan Matchett (936) 870-6187 or Brian Coleman (832) 567-3832.</Table.Caption>
            <Table.Header>
              <Table.Row>
                <Table.Head class="w-[200px]">Level</Table.Head>
                <Table.Head class="text-right">Amount</Table.Head>
              </Table.Row>
            </Table.Header>
            <Table.Body>
              <Table.Row>
                <Table.Cell class="font-medium">Title Sponsor</Table.Cell>
                <Table.Cell class="text-right">$10,000</Table.Cell>
              </Table.Row>
              <Table.Row>
                <Table.Cell class="font-medium">Platinum Sponsor</Table.Cell>
                <Table.Cell class="text-right">$5,000</Table.Cell>
              </Table.Row>
              <Table.Row>
                <Table.Cell class="font-medium">Gold Sponsor</Table.Cell>
                <Table.Cell class="text-right">$2,500</Table.Cell>
              </Table.Row>
              <Table.Row>
                <Table.Cell class="font-medium">Silver Sponsor</Table.Cell>
                <Table.Cell class="text-right">$1,000</Table.Cell>
              </Table.Row>
              <Table.Row>
                <Table.Cell class="font-medium">Trophy Sponsor</Table.Cell>
                <Table.Cell class="text-right">$100</Table.Cell>
              </Table.Row>
            </Table.Body>
          </Table.Root>
        </div>
    </div>
  </div>
</section>

<section class="container">
  <div class="max-w-[1000px] flex flex-col lg:flex-row items-center gap-10 mx-auto py-10">
    <div class="lg:max-w-[50%] md:max-w-[75%]">
      <img src="/CarShowAlvinMatthews.jpg" alt="sample_photo" class="">
    </div>
    <div class="text-left">
      <p class="tracking-wide ml-1">Subheader</p>
      <h2 class="text-3xl lg:text-4xl font-bold my-1">Another Text Section</h2>
      <p>Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat. Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.</p>
      <div class="border-l-2 pl-5 my-4">
        <p>April 6, 2024</p>
        <p>Rain Date April 13, 2024</p>
      </div>
    </div>
  </div>
</section>

<section class="container my-20">
  <div class="max-w-[1000px] items-center mx-auto gap-10">
    <Card.Root class="bg-accent text-center py-10">
      <Card.Header class="max-w-2xl mx-auto">
        <Card.Title class=" text-2xl capitalize">Get in touch</Card.Title>
        <Card.Description class=" text-lg">For more information, contact: Scott Harman (936) 870-8505, Jan Matchett (936) 870-6187 or Brian Coleman (832) 567-3832.</Card.Description>
      </Card.Header>
    </Card.Root>
  </div>
</section>  