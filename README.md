<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->

<h2>📌 Project Highlight: Hofstede's Cultural Alignment Test (Hofstede's CAT <img src="images/cat_emoji.png" width="2%"/>)</h2>

<h3>📖 Abstract:</h3>
<p>The deployment of large language models (LLMs) raises concerns regarding their cultural misalignment and potential ramifications on individuals and societies with diverse cultural backgrounds. While the discourse has focused mainly on political and social biases, our research proposes a Cultural Alignment Test (Hoftede's CAT) to quantify cultural alignment using Hofstede's cultural dimension framework, which offers an explanatory cross-cultural comparison through the latent variable analysis. We apply our approach to quantitatively evaluate LLMs—namely Llama 2, GPT-3.5, and GPT-4—against the cultural dimensions of regions like the United States, China, and Arab countries, using different prompting styles and exploring the effects of language-specific fine-tuning on the models' behavioural tendencies and cultural values. Our results quantify the cultural alignment of LLMs and reveal the difference between LLMs in explanatory cultural dimensions. Our study demonstrates that while all LLMs struggle to grasp cultural values, GPT-4 shows a unique capability to adapt to cultural nuances, particularly in Chinese settings. However, it faces challenges with American and Arab cultures. The research also highlights that fine-tuning LLama 2 models with different languages changes their responses to cultural questions, emphasizing the need for culturally diverse development in AI for worldwide acceptance and ethical use.</p>

<h3>🔍 Key Features of CAT:</h3>
<ul>
    <li><strong>Hofstede’s Framework:</strong> A trusted base for cross-cultural comparison.</li>
    <li><strong>In-depth Analysis:</strong> Coverage of diverse prompting styles and hyperparameter settings.</li>
    <li><strong>Quantifiable Metrics:</strong> Measures the cultural alignment of LLMs.</li>
</ul>

<h3>🌍 Cultures Analyzed:</h3>
<ul>
    <li>United States</li>
    <li>China</li>
    <li>Arab Countries</li>
</ul>

<h3>🔬 Methodology:</h3>
<p>The methodology behind Hofstede's CAT was designed to provide a quantifiable measure of cultural alignment in LLMs. Here's an overview of our approach:</p>
<ol>
    <li><strong>Framework Adoption:</strong> We began by integrating Hofstede’s cultural dimension framework to assess cultural alignment in LLMs, which involves 30 questions, including 24 on cultural dimensions and 6 on demographics. The ranking of these dimensions serves as a benchmark.</li>
    <li><strong>Prompting:</strong>
        <ol>
            <li><strong>Model Level:</strong> Assesses default cultural values in English, Chinese, and Arabic.</li>
            <li><strong>Country Level:</strong> Prompts LLMs in English to act like a person from specific countries.</li>
            <li><strong>Hyperparameter:</strong> Examines temperature and top-p settings in GPT-3.5.</li>
            <li><strong>Response Level:</strong> Analyzes consistency of responses.</li>
            <li><strong>Language Correlation:</strong> Compares cultural values of LLMs fine-tuned for English and Chinese.</li>
        </ol>
    </li>
    <li><strong>Cultural Dimensions:</strong> Six index scores are computed from the VSM13 responses.</li>
    <li><strong>Correlation and Misclassification:</strong> The Kendall Tau coefficient is used to rank correlations, and misclassification errors identify culturally misaligned countries.</li>
</ol>

<h3>🧪 Experiments:</h3>
<p>We evaluated the cultural alignment of three Large Language Models (LLMs): GPT-3.5, GPT-4, and Llama 2, focusing on the United States, China, and Arab countries, using Hofstede's cultural dimensions.</p>

<h4>Model Level Comparison:</h4>
<p>We compared the models' rankings with the original VSM13 values in English, Chinese, and Arabic:</p>
<ul>
  <li>GPT-4 outperforms GPT-3.5 in understanding and adapting to cultural nuances, showing superior performance without needing a specified persona.</li>
  <li>GPT-3.5 struggles with specific cultural nuances and shows poor adaptation when personas are used.</li>
</ul>

<h4>Country Level Comparison:</h4>
<p>We then assessed how the models performed when acting as individuals from specific countries:</p>
<ul>
  <li>GPT-4 shows better adaptability across different cultures, notably in the MAS (Masculinity vs. Femininity) dimension.</li>
  <li>Llama 2 and GPT-3.5 perform poorly when specific personas are involved in cultural contexts.</li>
  <li>The percentage of mis-ranked dimensions was highest for the United States.</li>
</ul>

<h4>Hyperparameter Comparison:</h4>
<p>We examined the impact of adjusting temperature and top-p settings in GPT-3.5 on cultural alignment:</p>
<ul>
  <li>Adjusting temperature and top-p settings significantly affects cultural alignment; lower temperature combined with either high top-p or moderate settings generally improves alignment.</li>
  <li>This highlights the importance of hyperparameters for cultural sensitivity.</li>
</ul>

<h4>Language Correlation:</h4>
<p>We compared Llama 2 models fine-tuned on English and Chinese:</p>
<ul>
  <li>There are notable differences in cultural reflections between English and Chinese models.</li>
  <li>The English models of both GPT-4 and LLama-2 tend to be more neutral, while the Chinese versions respond more positively.</li>
  <li>LLama-2's performance is generally lower compared to GPT models, with distinct variations between its English and Chinese versions.</li>
</ul>

<h3>📊 Results:</h3>
<ul>
  <li><strong>Performance Insights:</strong> Variability in GPT-4's cultural performance—poor in the U.S., better in China, problematic in Arab Countries.</li>
  <li><strong>Red-Teaming Effects:</strong> Suggests that the impact of red-teaming affects cultural sensitivity and performance of LLMs, with less red-teaming possibly benefiting performance in non-English contexts.</li>
  <li><strong>Ethical and Economic Impacts:</strong> Cultural misalignment risks ethical issues and economic setbacks, affecting AI's global trust and adoption.</li>
  <li><strong>Need:</strong> Culturally aligned AI is crucial for ethics, trust, and global adoption. This requires appropriate data, advanced techniques, interdisciplinary collaboration, and education.</li>
</ul>



<h3>📽️ Demo:</h3>
<p>Try out our demo on <a href="https://colab.research.google.com/drive/1dlPOpcRZhpxZU9pXbAuHzWGeFIneMadk#scrollTo=KmnbyU8f5VhG">Google Colab</a> to explore the cultural alignment of your desired LLMs.</p>

<!-- Collaborators section -->
<h3>🤝 Collaborators:</h3>
<ul>
    <li><a href="https://www.ee.ucl.ac.uk/iiml/members/masoud.html">Reem Masoud</a></li>
    <li><a href="https://sites.google.com/view/ziquanliu">Ziquan Liu</a></li>
    <li><a href="https://github.com/martinferianc">Martin Ferianc</a></li>
    <li><a href="http://www0.cs.ucl.ac.uk/staff/P.Treleaven/">Philip Treleaven</a></li>
    <li><a href="https://www.ucl.ac.uk/iccs/prof-miguel-rodrigues">Miguel Rodrigues</a></li>
    <!-- Add more as needed -->
</ul>


<h3>📄 Publication:</h3>
<ul>
    <li><a href="https://arxiv.org/abs/2309.12342">Cultural Alignment in Large Language Models:
An Explanatory Analysis Based on Hofstede’s Cultural
Dimensions</a></li>
</ul>

<h3>Citation</h3>
<pre><code>
@inproceedings{
masoud2024cultural,
title={Cultural Alignment in Large Language Models: An Explanatory Analysis Based on Hofstede's Cultural Dimensions},
author={Reem Masoud and Ziquan Liu and Martin Ferianc and Philip Colin Treleaven and Miguel R. D. Rodrigues},
booktitle={Global AI Cultures  @ ICLR 2024},
year={2024},
url={https://openreview.net/forum?id=HFt68VRiCb}
}
</code></pre>

<hr>

<p>
  🙏 Thank you for stopping by! Don't forget to ⭐️ star this repository if you find it interesting.
</p>

</body>

</html>
