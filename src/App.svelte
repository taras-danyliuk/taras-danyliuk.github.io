<script>
    import Row from "./components/Row.svelte";
    import Col from "./components/Col.svelte";

    import Experience from "./components/Experience.svelte";
    import Projects from "./components/Projects.svelte";
    import Education from "./components/Education.svelte";
    import Skills from "./components/Skills.svelte";
    import Contacts from "./components/Contacts.svelte";
</script>

<main>
    <Row>
        <Col span={16}>
            <div class="header">
                <h2>
                    JS
                    <br/>
                    Developer
                </h2>
                <h1>Taras Danyliuk</h1>
            </div>
        </Col>

        <Col span={8}>
            <img class="image" src="/profile_image.jpg" alt="Profile Image"/>
        </Col>
    </Row>

    <Row>
        <Col span={16}>
            <h3 class="section-title">Summary</h3>
            <p>5+ years of commercial experience in software development. Experience in leading teams, mentoring engineers and software architecture.</p>

            <Experience/>
            <Projects/>
            <Education/>
        </Col>

        <Col span={8}>
            <Skills/>
            <Contacts/>
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
        font-weight: 700;
        text-align: right;
        margin: 0;
    }

    :global(.section-title) {
        font-size: 1.75rem;
        line-height: 1.75rem;
        font-weight: 700;
        margin: 3rem 0 1rem;
    }

    @media (max-width: 750px) {
        .header {
            align-self: flex-end;
        }

        h1 {
            width: 100%;
            font-size: 2.5rem;
            line-height: 3rem;
            text-align: right;
            margin: 0;
        }

        h2 {
            margin: 0 0 1rem;
        }

        :global(.section-title) {
            font-size: 1.675rem;
            line-height: 1.675rem;
            margin: 1.5rem 0 0.5rem;
        }
    }

    @media print {
        .image {
            width: 45%;
        }
    }
</style>
