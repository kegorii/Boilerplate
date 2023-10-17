<script>
    import '../app.css';
    import beams from '$lib/assets/beams.jpg';
    import '@ibm/plex/css/ibm-plex-sans-kr.min.css';
</script>

<div class="relative flex min-h-screen flex-col justify-center overflow-hidden bg-gray-50 py-6 sm:py-12">
    <img src="{beams}" alt="" class="absolute top-1/2 left-1/2 max-w-none -translate-x-1/2 -translate-y-1/2" width="1308"/>
    <div class="absolute inset-0 bg-[url('$lib/assets/grid.svg')] bg-center [mask-image:linear-gradient(180deg,white,rgba(255,255,255,0))]"></div>
    <slot/>

</div>

