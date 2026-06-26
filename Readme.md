# AI-Top-Conf-JSONs

## 📝 About The Project

This project aims to systematically collect and organize the published paper metadata from top-tier conferences in Artificial Intelligence (AI), Computer Vision (CV), Natural Language Processing (NLP), and Machine Learning (ML).

To facilitate quick retrieval, statistical analysis, and secondary development for researchers and developers, all paper metadata is archived into folders by **Conference Name** and subsequently by **Year**. The data is uniformly extracted into a highly readable JSON format.

### 📄 Data Format Specification

Each JSON file represents a collection of papers for a specific conference in a given year. The data is stored in a dictionary (Key-Value) structure for simplicity:

- **Key**: The full title of the paper.
- **Value**: The corresponding official webpage link.


## 📂 Supported Conferences & Data Sources

This repository currently includes paper data from the following top-tier conferences. The specific details for each folder are as follows:

### 1. AAAI (Association for the Advancement of Artificial Intelligence)

- **📁 Folder:** `AAAI`
- **📅 Years Covered:** `2016 - 2026`
- **🔗 Official Data Source:** [AAAI Proceedings](https://ojs.aaai.org/index.php/AAAI/issue/archive)
- **📌 Included Tracks:** `All Main Technical Tracks`

### 2. ACL (Association for Computational Linguistics)

- **📁 Folder:** `ACL`
- **📅 Years Covered:** `2016 - 2026`
- **🔗 Official Data Source:** [ACL Proceedings](https://aclanthology.org/venues/acl/)
- **📌 Included Tracks:** `Main Conference (Long/Short Papers)`

### 3. CVPR (IEEE/CVF Conference on Computer Vision and Pattern Recognition)

- **📁 Folder:** `CVPR`
- **📅 Years Covered:** `2016 - 2026`
- **🔗 Official Data Source:** [CVF Open Access](https://openaccess.thecvf.com/menu)
- **📌 Included Tracks:** `Main Conference`

### 4. ECCV (European Conference on Computer Vision)

- **📁 Folder:** `ECCV`
- **📅 Years Covered:** `2018 - 2024 (even years)`
- **🔗 Official Data Source:** [ECCV Proceedings](https://www.ecva.net/papers.php)
- **📌 Included Tracks:** `Main Conference`

### 5. EMNLP (Empirical Methods in Natural Language Processing)

- **📁 Folder:** `EMNLP`
- **📅 Years Covered:** `2016 - 2025`
- **🔗 Official Data Source:** [EMNLP Proceedings](https://aclanthology.org/venues/emnlp/)
- **📌 Included Tracks:** `Main Conference`

### 6. ICCV (IEEE/CVF International Conference on Computer Vision)

- **📁 Folder:** `ICCV`
- **📅 Years Covered:** `2017 - 2025 (odd years)`
- **🔗 Official Data Source:** [CVF Open Access](https://openaccess.thecvf.com/menu)
- **📌 Included Tracks:** `Main Conference`

### 7. ICML (International Conference on Machine Learning)

- **📁 Folder:** `ICML`
- **📅 Years Covered:** `2016 - 2025`
- **🔗 Official Data Source:** [ICML Proceedings](https://proceedings.mlr.press/)
- **📌 Included Tracks:** `Main Conference`

### 8. IJCAI (International Joint Conference on Artificial Intelligence)

- **📁 Folder:** `IJCAI`
- **📅 Years Covered:** `2017 - 2025`
- **🔗 Official Data Source:** [IJCAI Proceedings](https://www.ijcai.org/all_proceedings)
- **📌 Included Tracks:** `Main Tracks`, `Survey Tracks (if available)`

### 9. NIPS / NeurIPS (Conference on Neural Information Processing Systems)

- **📁 Folder:** `NIPS`
- **📅 Years Covered:** `2016 - 2025`
- **🔗 Official Data Source:** [NeurIPS Proceedings](https://proceedings.neurips.cc/)
- **📌 Included Tracks:** `Main Conference`, `Datasets and Benchmarks (if available)`, `Position Papers (if available)`

## 🛠️ Quick Start

You can directly download the corresponding JSON files and easily parse them using Python:

```
import json

# Load CVPR 2026 paper data
with open('CVPR/cvpr_2026.json', 'r', encoding='utf-8') as f:
    papers = json.load(f)

# Print the first 5 papers
for title, url in list(papers.items())[:5]:
    print(f'Title: {title}\nURL: {url}\n')

```

## 📜 Disclaimer & License

This project only crawls and organizes publicly available, factual metadata (titles and public links) of academic papers. It does not contain full texts or abstracts protected by copyright. The final interpretation rights of all data belong to the official committees of the respective conferences.