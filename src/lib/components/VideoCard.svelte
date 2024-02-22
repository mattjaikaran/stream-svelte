<script lang="ts">
  import { Card, CardHeader, CardContent } from './ui/card';
  import Typography from './typography.svelte';
  import Badge from './ui/badge/badge.svelte';
  export let title: string;
  export let thumbnail: string = 'https://dummyimage.com/400x300/000/fff';
  export let views: string | number = 0;
  export let alt: string = 'Video Thumbnail';
  export let height: number = 300;
  export let width: number = 400;
</script>

<Card>
  <CardHeader>
    <img src={thumbnail} {alt} {width} {height} />
  </CardHeader>
  <CardContent>
    <Typography variant="h5" color="dark" classname="mb-2" text={title} />
    <p>Uploaded 2 days ago</p>
    <p>by Some User</p>
    <p>{views} views</p>
    <div class="mt-2">
      <Badge variant="default">Tag</Badge>
    </div>
  </CardContent>
</Card>
