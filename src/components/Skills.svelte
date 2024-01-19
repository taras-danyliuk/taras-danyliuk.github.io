<script>
    import Progress from "./Progress.svelte";
</script>

<div class="holder">
    <h3 class="section-title">Skills</h3>

    <p class="section">Front-end</p>
    <div class="row">
        <p class="title">JS</p>
        <Progress className="bar" width={70}/>
    </div>

    <div class="row">
        <p class="title">React.js</p>
        <Progress className="bar" width={80}/>
    </div>

    <div class="row">
        <p class="title">React Native</p>
        <Progress className="bar" width={80}/>
    </div>

    <div class="row">
        <p class="title">Next.js</p>
        <Progress className="bar" width={60}/>
    </div>

    <p class="section">Back-end</p>
    <div class="row">
        <p class="title">Node.js</p>
        <Progress className="bar" width={60}/>
    </div>

    <div class="row">
        <p class="title">Express.js</p>
        <Progress className="bar" width={60}/>
    </div>

    <div class="row">
        <p class="title">Meteor.js</p>
        <Progress className="bar" width={70}/>
    </div>

    <div class="row">
        <p class="title">MongoDB</p>
        <Progress className="bar" width={50}/>
    </div>

    <div class="row">
        <p class="title">PostgreSQL</p>
        <Progress className="bar" width={40}/>
    </div>
</div>

<style>
    .holder {
        width: 100%;
    }

    .section {
        font-weight: 800;
        color: #fff;
        font-size: 14px;
        margin: 5px 0;
    }

    .row {
        display: flex;
        align-items: center;
        margin: 5px 0;
    }

    .title {
        width: 40%;
        flex-shrink: 0;
        font-size: 14px;
    }
</style>
