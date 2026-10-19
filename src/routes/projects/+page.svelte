<script>
    import btdiagram from "#lib/assets/btinvest.png";
    import shocarlodiagram from '#lib/assets/shocarlo_text_formatter.png'
    import peakytype from '#lib/assets/led_display.png'
</script>

<style>
    a {
        color: saddlebrown;
    }
    a:hover {
        color: chocolate;
    }
    #ai-note {
        padding: 10px;
    }
    #ai-note h3 {
        padding-left: 10px;
        padding-right: 10px;
        margin: 5px;
    }
    #ai-note p {
        padding-left: 10px;
        padding-right: 10px;
        margin: 5px;
    }
    .project {
        border-width: 2px;
        border-color: black;
        border-style: solid;
        margin-top: 20px;
        margin-bottom: 20px;
    }
    .project h3 {
        position: relative;
        bottom: 17px;
        padding-left: 5px;
        padding-right: 5px;
        left: 7px;
        background: #fbf8f2;
        margin: 0;
        display: inline-block;
    }
    .project p {
        margin: 10px;
        margin-top: 0;
    }
</style>
<!--
<div id="ai-note">
    <hr>
    <h3>
       Note:
   </h3>
    <p>
        As AI has made large-scale software development much easier for inexperienced developers, the nature of what an
        impressive program to make has changed. I do not use AI in my development, not to discredit the usefulness of AI
        in the field, but because I enjoy learning software frameworks and building things myself. My projects instead
        stand as an example of how I am adaptable in learning new things, not as an example of how good I am at software
        development specifically. I enjoy the process of making, much as someone building their own furniture is not
        considering their cost-effectiveness to IKEA.
    </p>
    <hr>
</div> -->
<div class="project" style="margin-top: 33px;">
    <h3>
        bt-le-investigator
    </h3>
    <p>
        A two-part program with a client that captures nearby Bluetooth beacon frames and collects their MAC addresses,
        storing it in a database. A dashboard hosted on a server can then view these MAC addresses and associate them
        with devices and people for presence-detection.
    </p>
    <div class="attached-note" style="rotate: -0.5deg; height: 450px">
        <div class="staple1"></div>
        <div class="staple2"></div>
        <div class="staple3"></div>
        <div class="staple4"></div>
        <img src={btdiagram} alt="a diagram showing the design of the bt-investigator program">
    </div>
    <p style="text-align: right"><a href="https://github.com/beaubyte/bt-le-investigator">GitHub↗</a></p>
</div>
<div class="project">
    <h3>
        PeakyType
    </h3>
    <p>
        A hardware and software creation, this HUB75 led panel array driven by a Raspberry Pi 4 was
        diagrammed, wired, and programmed by me to be a multi-purpose interior LED sign. It connects to Discord
        and weather.gov APIs, renders fonts with an open-source library, and is frequently updated by
        me whenever I get new ideas.
    </p>
    <div class="attached-note" style="rotate: 0.2deg; height: 400px">
        <div class="staple1"></div>
        <div class="staple2"></div>
        <div class="staple3"></div>
        <div class="staple4"></div>
        <img src={peakytype} alt="a diagram showing the wiring of the peaky type">
    </div>
</div>
<div class="project">
    <h3>
        AirMedia Scripts
    </h3>
    <p>
        A set of AirMedia scripts written in Python that interact with the API to monitor, configure,
        and enforce large deployments of AirMedia 200 and 3000 devices. Future work on this project may
        use some console-driven interaction, including support for more Crestron devices at scale.
    </p>
</div>
<div class="project">
    <h3>
         shocarlo-text-formatter
    </h3>
    <p>
        An AI-enhanced serverless text formatter built in AWS that applies HTML rules and an LLM to
        achieve consistant text formatting on uploaded HTML documents and rich text.
    </p>
    <div class="attached-note" style="rotate: 0.3deg; height: 340px">
        <div class="staple1"></div>
        <div class="staple2"></div>
        <div class="staple3"></div>
        <div class="staple4"></div>
        <img src={shocarlodiagram} alt="a diagram showing the design of the shocarlo text formatter program">
    </div>
    <p style="text-align: right"><a href="https://github.com/beaubyte/shocarlo-text-formatter">GitHub↗</a></p>
</div>
<div class="project">
    <h3>
        PriceClicker
    </h3>
    <p>
        PriceClicker is a Java program built with the JavaFX framework. It is a basic cookie-clicker game around cafeteria food.
        It has a basic progression system, where you continue to click a burger and eventually can unlock things that
        will click for you, and items that will improve the value of each click you do. It can also write and load save
        data to a savefile.
    </p>
    <p style="text-align: right"><a href="https://github.com/beaubyte/PriceClicker">GitHub↗</a></p>
</div>
<div class="project">
    <h3>
        beaupod-loader
    </h3>
    <p>
        A script I made to get top songs from my Last.FM or from YouTube Music playlists/radios, attach metadata, and
        then download via yt-dlp to an .M4A file for loading onto my iPod. Requires a custom-compiled ffmpeg for proper
        codec support.
    </p>
    <p style="text-align: right"><a href="https://github.com/beaubyte/beaupod-loader">GitHub↗</a></p>
</div>
<div class="project">
    <h3>
        funye-vid-archiver
    </h3>
    <p>
        A Discord bot that gives the ability to archive videos from the internet and add them to an
        archive stored in a Discord channel and stored by Discord's CDN. Built to a very specific use-case,
        but performs very well under C++ as a systemd service.
    </p>
    <p style="text-align: right"><a href="https://github.com/beaubyte/funye-vid-archiver">GitHub↗</a></p>
</div>
<div class="project">
    <h3>
        timesavers
    </h3>
    <p>
        Timesavers is a website built for a TaaS (Time as a Service) company that sells the ability to go back in time
        to people. It offers premade places found it time to travel to, but also allows the ability to put in a custom
        order for a specific place in time. It uses PHP, HTML, CSS, MySQL, and JavaScript.
    </p>
    <p style="text-align: right;">
    <a href="https://github.com/beaubyte/timesavers" >GitHub↗</a>
    </p>
</div>
