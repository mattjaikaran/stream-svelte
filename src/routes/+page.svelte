<script lang="ts">
  import Typography from '$lib/components/typography.svelte';
  import {
    Carousel,
    CarouselContent,
    CarouselItem,
    Previous,
    Next
  } from '$lib/components/ui/carousel';
  import VideoCard from '$lib/components/VideoCard.svelte';
  import { homeData } from '$lib/home-data';
</script>

<main class="flex min-h-screen flex-col items-center justify-between p-16">
  <Carousel>
    <CarouselContent>
      <CarouselItem>
        <img
          src="https://dummyimage.com/2000x500/000/fff"
          alt="Video Streaming App"
          width={2000}
          height={500}
        />
      </CarouselItem>
      <CarouselItem>
        <img
          src="https://dummyimage.com/2000x500/f2f2f2/000"
          alt="Video Streaming App"
          width={2000}
          height={500}
        />
      </CarouselItem>
    </CarouselContent>
    <Previous />
    <Next />
  </Carousel>
  <Typography variant="h5" color="dark" classname="my-4" text="Cool Featured Content" />
  <div class="grid gap-4 lg:grid-cols-3">
    <VideoCard title="here is some text" />
    <VideoCard title="here is some text" />
    <VideoCard title="here is some text" />
  </div>

  <Typography variant="h5" color="dark" classname="my-4" text="Featured Videos" />
  <div class="grid gap-4 lg:grid-cols-3">
    {#each homeData as video}
      <VideoCard title={video.title} thumbnail={video.thumbnail} views={video.views} />
    {/each}
  </div>

  <Typography variant="h5" color="dark" classname="my-4" text="Live Streams" />
  <Carousel>
    <CarouselContent>
      <CarouselItem>
        <div class="grid gap-4 lg:grid-cols-4">
          <VideoCard title="carousel text1" />
          <VideoCard title="carousel text1" />
          <VideoCard title="carousel text1" />
          <VideoCard title="carousel text1" />
        </div>
      </CarouselItem>
      <CarouselItem>
        <div class="grid gap-4 lg:grid-cols-4">
          <VideoCard title="carousel text2" />
          <VideoCard title="carousel text2" />
          <VideoCard title="carousel text2" />
          <VideoCard title="carousel text2" />
        </div>
      </CarouselItem>
    </CarouselContent>
    <Previous />
    <Next />
  </Carousel>
</main>
