---
layout: about
---

## About Me

I am a second year CS PhD student at [Khoury College of Computer Science](https://www.khoury.northeastern.edu/) at Northeastern University in Boston. I am advised by [Prof Mai ElSherief](https://www.maielsherief.com/).

Before starting my PhD, I was a Software Engineer with the [Selection Monitoring and Catalog Systems](https://www.amazon.jobs/content/en/teams/e-commerce-foundation/ascs) organization at Amazon in Seattle. Prior to that I was an MS CS student at [Georgia Tech](https://www.gatech.edu/). At Georgia Tech, I was advised by [Prof Srijan Kumar](https://faculty.cc.gatech.edu/~srijan/) in the CLAWS Lab. I also dabble as a Research mentor with [SimPPL](https://simppl.org/).

## Publications


<!-- Filtering controls -->
<select id="filter-year">
  <option value="all">All Years</option>
  <option value="2025">2025</option>
  <option value="2023">2023</option>
  <option value="2021">2021</option>
  <option value="2020">2020</option>
</select>

<select id="filter-conference">
  <option value="all">All Conferences</option>
  <option value="EMNLP Findings">EMNLP Findings</option>
  <option value="NeurIPS SafeGenAI">NeurIPS SafeGenAI</option>
  <option value="arXiv">arXiv</option>
  <option value="ITM Web Conf">ITM Web Conf</option>
  <option value="Elsevier">Elsevier</option>
  <option value="IJCA">IJCA</option>
</select>

<div class="publications">

<div class="publication" data-year="2025" data-conference="EMNLP Findings">
- **Malik, Ananya**, Nazanin Sabri, Melissa Karnaze, and Mai Elsherief.  
  *Are LLMs Empathetic to All? Investigating the Influence of Multi-Demographic Personas on a Model's Empathy.*  
  _EMNLP Findings 2025._  
  [📄 Paper Link](https://arxiv.org/pdf/2510.10328)
</div>

<!-- (other publications here with same data-year/data-conference attributes) -->

</div>

<script>
const yearFilter = document.getElementById('filter-year');
const confFilter = document.getElementById('filter-conference');
const pubs = document.querySelectorAll('.publication');

function applyFilters() {
  const year = yearFilter.value;
  const conf = confFilter.value;
  pubs.forEach(pub => {
    const matchYear = (year === 'all' || pub.dataset.year === year);
    const matchConf = (conf === 'all' || pub.dataset.conference === conf);
    pub.style.display = (matchYear && matchConf) ? 'block' : 'none';
  });
}

yearFilter.addEventListener('change', applyFilters);
confFilter.addEventListener('change', applyFilters);
</script>


## Research Interest

I am interested in designing, evaluating, and aligning AI systems to maximize social benefit while minimizing risks. My work sits at the intersection of natural language processing (NLP), AI alignment, AI safety, and the study of online communities, with a focus on how AI can be more empathetic, fair, and socially aware.

### 🤖👤 AI Safety and Personalization

I deeply interested in studying how LLMs behave and can be made safer and more aligned. My past work has investigated the impact of incorporating user personas and contextual information in the model's behaviour, value alignment, and empathetic capabilities [TBD]. I have been able to explore this impact through both [explicit personas of genders](https://arxiv.org/pdf/2311.14788)) as well as the effect of implicit user personas through dialect [(SafeGenAI Oral Presentation @ NeurIPS'24)](https://arxiv.org/abs/2410.20490). Recently, I have been investigating how the addition of personas and contextual signals into large language models can guide their behavior toward safer, value-aligned outputs.

My ongoing work with [Geodesic Research](https://www.geodesicresearch.org/) @ MARS has been exploring different and internal pathways toward AI control, more on that coming soon!

### 🤖🤝✨ Value Based Alignment

I am interested in studying how we can align models with human values, with a particular focus on maintaining emotional safety. In my recent work (to appear in EMNLP 2025; paper coming soon 👀), we found that models are highly influenced by a user’s context, often resulting in disproportionate variation in their empathetic capabilities. A further deep dive, conducted by Bangzhao Shu in a paper currently under submission, shows that models express emotions in ways that differ systematically from human emotional expression. Building on these findings, I am exploring ways to reduce this divergence and develop methods that make models emotionally safe, ensuring their responses are consistent, empathetic, and aligned with human expectations.

### 🤝🌐 Understanding and Analyzing for Social Good Applications

In the past, I have studied how AI can support healthier online communities. This includes analyzing misinformation on social media, categorizing [hate speech reasoning](https://ananyamalikk.substack.com/p/intent-to-hate), and [identifying dog whistles](https://drive.google.com/file/d/1hYIJjy92jo9VgBmfIY3AZTr-KUbr0dTa/view). These projects aim to create actionable tools and interventions that make digital spaces safer, more inclusive, and resilient, combining technical research with real-world social impact.


## Academic Service and Groups

### Groups 

- [CSG (Computation for Social Good) Lab @ NEU](https://www.maielsherief.com/)
- [Geodesic Research](https://www.geodesicresearch.org/)
- [MAIA](https://aialignment.mit.edu/)
- [SimPPL](https://simppl.org/)
- [CLAWS](https://faculty.cc.gatech.edu/~srijan/)

### Teaching

- TA for [CS 5200: Database Management Systems](https://www.khoury.northeastern.edu/people/martin-schedlbauer/)
-  TA for [CS 4100: Foundations of AI (Spring 2025)](https://www.khoury.northeastern.edu/home/camato/4100summaryS25.html) with Prof Chris Amato

- TA for CS 3600: Intro to AI, with Prof James Rehg (Spring 2022) and Prof Mark Reidl (Fall 2022)

### Talks

- [Slides](https://www.canva.com/design/DAGjgwNOPBE/Z09A59smG8vXAGvgaW7PFA/view?utm_content=DAGjgwNOPBE&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h7faf8a8774) of my lecture on Advanced Topics in AI

- Presentation and Slides at SafeGenAI workship at NeurIPS on [Who Speaks Matters: Analysing the Influence of the Speaker’s Ethnicity on Hate Classification](https://neurips.cc/virtual/2024/workshop/84705#wse-detail-109375)