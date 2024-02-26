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
    import { AspectRatio } from "$lib/components/ui/aspect-ratio";
  </script>
  
  <header class="py-5 container z-10 max-w-[1100px]">
    <div id="header-inner" class="flex flex-col sm:flex-row gap-8 justify-between items-center ml-auto">
      <div id="site-title" class="text-center sm:text-left">
        <a href="/" class="flex flex-row items-center gap-4 justify-center sm:justify-start">
          <img class="max-w-14 inline-block" src="/RichardsLodge1116Logo.webp" alt="Richards Lodge 1116 Logo">
          <div >Richards Lodge 1116</div>
        </a>
      </div>
      
    </div>
  </header>
  
  <section class="my-10">
    <div class="container max-w-[1200px]">
      <div class="flex flex-row ml-auto lg:gap-20 gap-5">
        <div class="md:max-w-[60%] z-10 text-left">
          <h2 class="lg:text-xl my-2 tracking-wider text-nowrap">
            <span class="uppercase bg-primary text-primary-foreground px-4 py-2 rounded-md font-semibold leading-10">16th Annual Richards Lodge 1116</span><br>
            <span class="text-6xl md:text-8xl leading-tight font-bold">Car Show <br><span class="text-ring">&</span> Fundraiser</span>
          </h2>
          <p class="lg:text-xl lg:my-3 max-w-[90%] leading-relaxed">Join us at Yankee's Tavern in Carlos, Texas on April 6, 2024. Proceeds from this event go to support the local charities and communities in need that Richards Lodge is actively involved with.</p>
        </div>
        <div class="">
          <!-- <div class="absolute top-60 -right-4 w-96 h-72 bg-yellow-400 rounded-full filter blur-2xl mix-blend-screen "></div> -->
          <div class="absolute hidden dark:block top-10 -right-30 w-[50%] h-[700px] bg-primary rounded-full filter blur-3xl opacity-30 mix-blend-screen"></div>
          <img src="/carshow-hero.webp" alt="car show" class="z-5 hidden lg:block absolute lg:w-[600px] md:w-[33%] md:top-20 lg:top-12 right-0 drop-shadow-2xl">
        </div>
      </div>
    </div>
  </section>
  
  <section class="lg:mt-60 mt-10 container">
    <div class="max-w-[1200px] mx-auto">
      <div class="relative">
        <div class="absolute hidden dark:block top-0 -left-60 w-[80%] h-[700px] bg-primary rounded-full filter blur-3xl opacity-10 mix-blend-screen"></div>
      </div>
      <p class="text-[5vw] text-nowrap font-bold lg:text-6xl "><span class="bg-primary text-primary-foreground px-3 rounded-md">Food</span> • <span class="bg-primary text-primary-foreground px-3 rounded-md">Music</span> <span class="text-accent-foreground">•</span> <span class="bg-primary px-3 text-primary-foreground rounded-md">Door Prizes</span></p>
      <ul class="text-lg lg:text-4xl lg:mt-10 mt-5 capitalize">
        <li class="mb-4">⭐️ Open to the public</li>
        <li class="mb-4">⭐️ Doors Open at 8:00 AM</li>
        <li class="mb-4">⭐️ Registration is open from 8:00 AM to 12:00 PM</li>
        <li class="mb-4">⭐️ Awards presentation is at 2:00 PM</li>
        <li class="mb-4">⭐️ 25 awards for cars, trucks, jeeps, and bikes</li>
      </ul>
    </div>
  </section>

  <section class="my-20 container max-w-[1100px]">
  <AspectRatio ratio={21 / 9} class="bg-muted">
    <img
      src="/RedSilver.jpg"
      alt="Gray by Drew Beamer"
      class="h-full w-full rounded-md object-cover"
    />
  </AspectRatio>
</section>

  
  <section class="container my-36">
    <div class="relative">
      <div class="absolute hidden dark:block z-0 -top-32 -right-60 w-[80%] h-[700px] bg-primary rounded-full filter blur-3xl opacity-10 mix-blend-screen"></div>
    </div>
    <div class="mx-auto z-1 text-center my-10">
      <h2 class="lg:text-6xl text-3xl text-center font-semibold my-2">Sponsorship Opportunities</h2>
      <p class="max-w-[600px] mx-auto mt-8">Our sponsors are so important... Lorem ipsum dolor sit amet, qui minim labore adipisicing... This how it works:</p>
    </div>
    <div class="overflow-x-auto">
      <div class="max-w-[800px] mx-auto">
        <div class="max-w-[500px] mx-auto">
            <Table.Root class="text-xl">
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
      <div class="">
          <img src="/CarShowAlvinMatthews.jpg" alt="sample_photo" class="rounded-md">
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
          <Card.Title class=" text-3xl mb-5 capitalize">Get in touch</Card.Title>
          <Card.Description class=" text-lg">For more information, contact: Scott Harman (936) 870-8505, Jan Matchett (936) 870-6187 or Brian Coleman (832) 567-3832.</Card.Description>
        </Card.Header>
      </Card.Root>
    </div>
  </section>  

  <div class="fixed bottom-0 right-0 ml-auto">
    <div id="theme-toggle">
      <Button on:click={toggleMode} variant="outline" size="icon">
        <Sun class="h-[1.2rem] w-[1.2rem] rotate-0 scale-100 transition-all dark:-rotate-90 dark:scale-0" />
        <Moon class="absolute h-[1.2rem] w-[1.2rem] rotate-90 scale-0 transition-all dark:rotate-0 dark:scale-100" />
        <span class="sr-only">Toggle theme</span>
      </Button>
    </div>
  </div>