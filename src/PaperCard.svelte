<script>
     import Card, {
    Content,
    PrimaryAction,
    Media,
    MediaContent,
  } from '@smui/card';
</script>


<div class="card-container">
    <Card style="min-width: 300px;">
      <Media class="card-media-square" aspectRatio="square">
        <div style="color: #fff; position: absolute; bottom: 16px; left: 16px;">
          <h2 class="mdc-typography--headline6" style="margin: 0;">
            A card with square media.
          </h2>
          <h3 class="mdc-typography--subtitle2" style="margin: 0;">
            And a subtitle.
          </h3>
        </div>
      </Media>
    </Card>
  </div>


<style>
    * :global(.card-media-16x9) {
      background-image: url(https://place-hold.it/320x180?text=16x9&fontsize=23);
    }
   
    * :global(.card-media-square) {
      background-image: url(https://place-hold.it/320x320?text=square&fontsize=23);
    }
  </style>