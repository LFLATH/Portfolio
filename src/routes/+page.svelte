<script>
    import Logo from "../components/logo.svelte";
    import Hero from "../components/hero.svelte";
    import Experience from "../components/experience.svelte"
    import Section from "../components/section.svelte";
    import LinkCard from "../components/link_card.svelte";
    




    let fas_title = "Software Engineering Intern,   May 2023 - August 2023"
    let fas_desc = [
        "Developed middleware scripts to transform order data stored in Microsoft SQL Server into data that could be displayed on an HMI",
        "Designed and implemented an internal asset management system using Winform and C# that improved accuracy and efficiency in accounting ", "Deployed testing programs for SCADA systems to PLCs"
    ]
    let gt_date = "August 2022 - December 2024"
    /**
     * @type {never[]}
     */
    let gt_desc = []
</script>


<div class="page_container">
    <Logo></Logo>
    <Hero></Hero>
    <div class="heading_container">
        <Section 
        heading = {"Experience"}
        --color = #444795
        />
    </div> 
    <div class="experience_container">
        <Experience 
        image={"/images/fas.png"}
        company={"Factory Automation Systems"}
        title_date = {fas_title}
        desc = {fas_desc}
        --img_width= 28em
        --img_height= 24em
        />
    </div>
    <div class="heading_container">
        <Section 
        heading = {"Education"}
        --color = #E74536
        />
    </div> 
    <div class="education_container">
        <Experience 
            image={"/images/gt.png"}
            company={"Georgia Institute of Technology"}
            title_date = {gt_date}
            desc = {gt_desc}
            --img_width= 28em
            --img_height= 24em
            /> 
    </div>
    <div class="heading_container">
        <Section 
        heading = {"Links"}
        --color = #FFC915
        />
    </div>
    <div class="links_container">
        <LinkCard
        image={"/images/github.png"}
        link_name={"Github"}
        link={"https://github.com/LFLATH"}
        />
        <LinkCard
        image={"/images/linkedin.png"}
        link_name={"Linkedin"}
        link={"https://www.linkedin.com/in/ludwig-lechtreck-884a34212/"}
        />
        <LinkCard
        image={"/images/resume.png"}
        link_name={"Resume"}
        link={"/images/Resume.pdf"}
        />
    </div>
    
</div>



<style>
    .page_container {
        font-family: 'Baumans', cursive;;
    }
    .page_container {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
    }
    .experience_container {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
    }
    .heading_container {
        text-align: center;
        padding-bottom: 2em;
    }
    .education_container {
        display: flex;
        flex-direction: row;
        justify-content: center;
    }
    .links_container {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
    }

</style>