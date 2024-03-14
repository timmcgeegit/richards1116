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
    import * as Accordion from "$lib/components/ui/accordion";
	import TableRow from "$lib/components/ui/table/table-row.svelte";
  </script>
  
  <header class="py-5 container z-10">
    <div id="header-inner" class="flex flex-col sm:flex-row gap-8 justify-between items-center ml-auto max-w-[1200px]">
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
            <span class="uppercase text-nowrap text-primary px-2 py-2 rounded-md font-bold leading-loose">16th Annual Richards Lodge 1116</span><br>
             <span class="text-5xl text-nowrap md:text-8xl leading-tight font-bold">Car Show <br><span class="text-ring">&</span> Fundraiser</span>
          </h2>
          <p class="lg:text-xl lg:my-3 leading-relaxed">Join us at Yankee's Tavern in Carlos, Texas on April 6, 2024 (Rain Date April 13, 2024). Proceeds from this event go to support scholarships for local seniors, local charities, Richards Lodge, and communities that Richards Lodge is actively involved with.</p>
        </div>
        <div class="hidden lg:block">
          <!-- <div class="absolute top-60 -right-4 w-96 h-72 bg-yellow-400 rounded-full filter blur-2xl mix-blend-screen "></div> -->
          <div class="absolute hidden flex overflow-hidden dark:block top-10 right-0 w-[50%] h-[1000px] bg-primary rounded-full filter blur-3xl opacity-10 mix-blend-screen"></div>
          <img src="/CarShowGeneGallin.jpg" alt="Picture of red car at a car show" class="rounded"> 
          
        </div>
      </div>
    </div>
  </section>
  
  <section class="lg:my-32 mt-10 container">
    <div class="max-w-[1200px] mx-auto">
      <div class="relative">
        <div class="absolute hidden overflow-hidden dark:block top-0 -left-60 w-[80%] h-[700px] bg-primary rounded-full filter blur-3xl opacity-10 mix-blend-screen"></div>
      </div>
      <p class="text-[5vw] text-nowrap font-bold lg:text-6xl "><span class="bg-primary text-primary-foreground px-3 rounded-md">Food</span> • <span class="bg-primary text-primary-foreground px-3 rounded-md">Music</span> <span class="text-accent-foreground">•</span> <span class="bg-primary px-3 text-primary-foreground rounded-md">Door Prizes</span></p>
      <ul class="text-lg lg:text-4xl lg:mt-10 mt-5 capitalize">
        <li class="lg:mb-4">⭐️ Open to the public</li>
        <li class="lg:mb-4">⭐️ Doors Open at 8:00 AM</li>
        <li class="lg:mb-4">⭐️ Registration is open from 8:00 AM to 12:00 PM</li>
        <li class="lg:mb-4">⭐️ Awards presentation is at 2:00 PM</li>
        <li class="lg:mb-4">⭐️ 25 awards for cars, trucks, jeeps, and bikes</li>
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
    <p class="max-w-2xl text-lg mx-auto mt-8">
      Our sponsors are so important. Thank you for your continued investment in the community in which we all live and work. Click each sponsorship level to learn more: 
    </p>
  </div>
  <div class="overflow-x-auto">
    <div class="max-w-[800px] mx-auto">
      <div class="">
        <Table.Root class="text-xl">
          <Table.Caption class="max-w-3xl text-lg mx-auto">
            Make checks payable to "Richards Lodge 1116" and send them to P.O. Box 404 Richards, Texas 77873.
            For more information, contact: Jan Matchett (936) 870-6187, Brian Coleman (832) 567-3832 or Perry Palmer (281) 468-8118
          </Table.Caption>
          <Table.Header>
          <Table.Row>
          <Table.Head class="">Level</Table.Head>
          <Table.Head class="text-right pr-8">Amount</Table.Head>
          </Table.Row>
          </Table.Header>
          <Table.Body>
            <Table.Row>
            <Table.Cell colspan="2">
            <Accordion.Root>
            <Accordion.Item value="item-1">
            <Accordion.Trigger class="flex justify-between decoration-transparent items-center w-full text-xl font-medium">
            <span>Title Sponsor</span>
            <span class="ml-auto pr-2">$10,000</span>
            </Accordion.Trigger>
            <Accordion.Content>
              Your Title Sponsorship will include banner signage at the car show as well as on the 2024 website and in years to come. 500 free door prize tickets and lunch for you and your guests. Free Car registration for all your entries. Also includes the opportunity to speak to all attendees at the awards presentation.
            </Accordion.Content>
            </Accordion.Item>
            </Accordion.Root>
            </Table.Cell>
            </Table.Row>
            <Table.Row>
              <Table.Cell colspan="2">
              <Accordion.Root>
              <Accordion.Item value="item-1">
              <Accordion.Trigger class="flex justify-between decoration-transparent items-center w-full text-xl font-medium">
              <span>Platinum Sponsor</span>
              <span class="ml-auto pr-2">$5,000</span>
              </Accordion.Trigger>
              <Accordion.Content>
                Your Platinum Sponsorship will include banner signage at the car show as well as on the 2024 website and in years to come. 200 free door prize tickets and lunch for you and 10 guests. Free Car registration for all your entries. Also includes the opportunity to speak to all attendees at the awards presentation.
              </Accordion.Content>
              </Accordion.Item>
              </Accordion.Root>
              </Table.Cell>
              </Table.Row>
              <Table.Row>
                <Table.Cell colspan="2">
                <Accordion.Root>
                <Accordion.Item value="item-1">
                <Accordion.Trigger class="flex justify-between decoration-transparent items-center w-full text-xl font-medium">
                <span>Gold Sponsor</span>
                <span class="ml-auto pr-2">$2,500</span>
                </Accordion.Trigger>
                <Accordion.Content>
                  Your Gold Sponsorship will include banner signage at the car show as well as on the 2024 website and in years to come. 100 free door prize tickets and lunch for you and 4 guests. Free Car registration for up to 8 entries.
                </Accordion.Content>
                </Accordion.Item>
                </Accordion.Root>
                </Table.Cell>
                </Table.Row>
                <Table.Row>
                  <Table.Cell colspan="2">
                  <Accordion.Root>
                  <Accordion.Item value="item-1">
                  <Accordion.Trigger class="flex justify-between decoration-transparent items-center w-full text-xl font-medium">
                  <span>Silver Sponsor</span>
                  <span class="ml-auto pr-2">$1,000</span>
                  </Accordion.Trigger>
                  <Accordion.Content>
                    Your Silver Sponsorship will include banner signage at the car show as well as on the 2024 website and in years to come. 50 free door prize tickets and lunch for you and 2 guests. Free Car registration for up to 4 entries.
                  </Accordion.Content>
                  </Accordion.Item>
                  </Accordion.Root>
                  </Table.Cell>
                  </Table.Row>
                  <Table.Row>
                    <Table.Cell colspan="2">
                    <Accordion.Root>
                    <Accordion.Item value="item-1">
                    <Accordion.Trigger class="flex justify-between decoration-transparent items-center w-full text-xl font-medium">
                    <span>Trophy Sponsor</span>
                    <span class="ml-auto pr-2">$100</span>
                    </Accordion.Trigger>
                    <Accordion.Content>
                      Your Trophy Sponsorship will include banner signage at the car show as well as on the 2024 website and in years to come.
                    </Accordion.Content>
                    </Accordion.Item>
                    </Accordion.Root>
                    </Table.Cell>
                    </Table.Row>
          </Table.Body>
          </Table.Root>
      </div>
    </div>
  </div>
</section>
  
  <section class="container my-20">
    <div class="max-w-[1000px] items-center mx-auto gap-10">
      <Card.Root class="bg-accent text-center py-10">
        <Card.Header class="max-w-2xl mx-auto">
          <Card.Title class=" text-3xl mb-5 capitalize">Get in touch</Card.Title>
          <Card.Description class=" text-lg">For more information, contact: Jan Matchett (936) 870-6187, Brian Coleman (832) 567-3832 or Perry Palmer (281) 468-8118 </Card.Description>
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