<script>
    import Row from "./Row.svelte";
    import Col from "./Col.svelte";
    import Icon from "svelte-awesome";
    import { github, linkedin, envelopeO } from "svelte-awesome/icons";
</script>

<div>
    <h3 class="section-title">Contacts</h3>

    <Row>
        <Col span={3} responsive={false}>
            <Icon data={github} scale={1.5}/>
        </Col>
        <Col span={21} justifyContent="center" responsive={false}>
            <a href="https://github.com/taras-danyliuk/" target="_blank">taras-danyliuk</a>
        </Col>
    </Row>

    <Row>
        <Col span={3} responsive={false}>
            <Icon data={linkedin} scale={1.5}/>
        </Col>
        <Col span={21} justifyContent="center" responsive={false}>
            <a href="https://www.linkedin.com/in/taras-danyliuk-832178109" target="_blank">Taras Danyliuk</a>
        </Col>
    </Row>

    <Row>
        <Col span={3} responsive={false}>
            <Icon data={envelopeO} scale={1.5}/>
        </Col>
        <Col span={21} justifyContent="center" responsive={false}>
            <a href="mailto:tarik.danylyuk@gmail.com">tarik.danylyuk@gmail.com</a>
        </Col>
    </Row>
</div>

<style>
    a {
        font-size: 12px;
        margin-left: 10px;
    }
</style>
