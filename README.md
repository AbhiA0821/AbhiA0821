from pathlib import Path
from textwrap import dedent
from pypandoc import convert_text

md = dedent(r"""
<div align="center">

# 👋 Hi, I'm Abhishek Ainapure

### AI Engineer • Data Engineering Enthusiast • Machine Learning

<img src="https://readme-typing-svg.demolab.com?font=Poppins&size=24&duration=3000&pause=1000&center=true&vCenter=true&width=700&lines=Artificial+Intelligence+%26+Data+Science;AI+Engineer;Data+Engineering+Enthusiast;PySpark+%7C+DuckDB+%7C+Airflow;Generative+AI+%7C+LLMs" />

</div>

---

## 👨‍💻 About Me

- 🎓 B.Tech in Artificial Intelligence & Data Science
- 🤖 Passionate about AI, Machine Learning & Data Engineering
- 🌱 Currently learning **PySpark, DuckDB, Apache Airflow & LLMs**
- 🚀 Building real-world AI projects including **MedIntel**
- 📍 Maharashtra, India

---

## 🛠 Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

**Data Engineering**

![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)

**AI & ML**

![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

---

## 🚀 Featured Projects

- 🏥 **MedIntel** – AI Healthcare Data Pipeline using PySpark, DuckDB, Airflow & LLMs.
- 📄 **AI Resume Analyzer** – Resume matching using ML.
- 🎨 **Ghibli Image Generator** – CycleGAN-based image generation.

---

## 📊 GitHub Analytics

<p align="center">
<img height="165" src="https://github-readme-stats.vercel.app/api?username=AbhiA0821&show_icons=true&theme=tokyonight&hide_border=true"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AbhiA0821&layout=compact&theme=tokyonight&hide_border=true"/>
</p>

<p align="center">
<img src="https://streak-stats.demolab.com?user=AbhiA0821&theme=tokyonight&hide_border=true"/>
</p>

<p align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=AbhiA0821&theme=tokyo-night&hide_border=true"/>
</p>

---

## 🤝 Connect With Me

[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ainapureabhi0821@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishek-ainapure)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AbhiA0821)

---

## 🐍 Contribution Snake

> Add the generated snake SVG after enabling the GitHub Actions workflow.

---

<div align="center">

⭐ *Thanks for visiting my profile!*

</div>
""")

out = Path("/mnt/data/README.md")
convert_text(md, "md", format="md", outputfile=str(out), extra_args=["--standalone"])
print(out)
