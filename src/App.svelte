<script>
    import Row from "./components/Row.svelte";
    import Col from "./components/Col.svelte";
    import Icon from "svelte-awesome";
    import { github, linkedin, envelopeO } from 'svelte-awesome/icons';
</script>

<main>
    <Row>
        <Col span={16}>
            <div class="header">
                <h1>Taras Danyliuk</h1>
                <h2>JS Developer</h2>
            </div>
        </Col>

        <Col span={8}>
            <img src="/profile_image.jpg" alt="Profile Image"/>
        </Col>
    </Row>

    <Row>
        <Col span={16}>
            <h3 class="section-title">Summary</h3>
            <p>5+ years of commercial experience in software development. Experience in leading teams, mentoring engineers and software architecture.</p>

            <h3 class="section-title">Experience</h3>
            <h3 class="section-title">Projects</h3>
            <h3 class="section-title">Education</h3>
            <h3 class="section-title">Skills</h3>
        </Col>

        <Col span={8}>
            <h3 class="section-title">Contacts</h3>

            <Row>
                <Col span={3}>
                    <Icon data={github} scale={1.5}/>
                </Col>
                <Col span={21}>
                    <a href="https://github.com/taras-danyliuk/" target="_blank">taras-danyliuk</a>
                </Col>
            </Row>

            <Row>
                <Col span={3}>
                    <Icon data={linkedin} scale={1.5}/>
                </Col>
                <Col span={21}>
                    <a href="https://www.linkedin.com/in/taras-danyliuk-832178109" target="_blank">Taras Danyliuk</a>
                </Col>
            </Row>

            <Row>
                <Col span={3}>
                    <Icon data={envelopeO} scale={1.5}/>
                </Col>
                <Col span={21}>
                    <a href="mailto:tarik.danylyuk@gmail.com">tarik.danylyuk@gmail.com</a>
                </Col>
            </Row>
        </Col>
    </Row>
</main>


<style>
    .header {
        align-self: flex-start;
    }

    img {
        width: 100%;
        align-self: flex-end;
    }

    h1 {
        text-transform: uppercase;
        font-size: 3.5rem;
        line-height: 3.5rem;
        font-weight: 800;
        letter-spacing: -0.1rem;
        margin: 0 0 0.5rem;
    }

    h2 {
        font-size: 1.5rem;
        line-height: 1.5rem;
        font-weight: 400;
        text-align: right;
        margin: 0;
    }

    .section-title {
        font-size: 1.75rem;
        line-height: 1.75rem;
        font-weight: 700;
        margin: 2rem 0 1rem;
    }

    @media (max-width: 750px) {
        .header {
            align-self: flex-end;
        }

        h1 {
            width: 100%;
            font-size: 2.5rem;
            line-height: 3rem;
            text-align: center;
            margin: 0;
        }

        h2 {
            text-align: right;
            margin: 0 0 1rem;
        }

        .section-title {
            font-size: 1.675rem;
            line-height: 1.675rem;
            margin: 1rem 0 0.5rem;
        }
    }
</style>
