---
layout: page
title: Faculty Members
permalink: /faculty/
---

[Ben Tyler](/faculty/tyler)

[Mona Rizvi](/faculty/rizvi) 

[Martin Lukac](/faculty/lukac) 

[Anotnio Cerone](/faculty/cerone) 

[Michael Lewis](/faculty/lewis) 

[Mark Sterling](/faculty/sterling) 

[Askar Boranbayev](/faculty/boranbayev) 

[Bolatzhan Kumalakov](/faculty/kumalakov)

[Sain Saginbekov](/faculty/saginbekov)






<style>
.content {
    display: none;
}
</style>
<script>
$(".header").click(function () {

    $header = $(this);
    //getting the next element
    $content = $header.next();
    //open up the content needed - toggle the slide- if visible, slide up, if not slidedown.
    $content.slideToggle(500, function () {
        //execute this after slideToggle is done
        //change text of header based on visibility of content div
        $header.text(function () {
            //change text based on condition
            return $content.is(":visible") ? $header.text().substr(0, $header.text().length-6)+"[-]   " : $header.text().substr(0, $header.text().length-6)+"[+]   ";
        });
    });

});
</script>
