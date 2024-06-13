# 2024 Resume

# Jeffrey Lin (林奕勳)

ESUN Bank, Intelligent Finance Technology Department, AI Engineer focusing on building ML and Data Products and Frameworks.

jeffrey82221@gmail.com TW, Taipei

## CAREER SUMMARY

6+ years of python software design experience, focusing on large-scale AI product development, specialized in the design of developer framework, SDK, and testing methods for optimizing the research/deployment flow of data science, ETL, and machine learning pipelines.

4+ years of financial AI development experience, as the developer, product owner, and techical leader of data science department, participate in the prototyping, evaluation, and deployment phase of various data products, including house price and credit loan estimation services, and 360 degree customer knowledge graph data services.

2+ year of participation in the technology management assistant bootcamp, with real-experience on business user support, gaining first-hand insight on financial and corporative AI usage via cross-department collaboration.

Having excellent code-quality standard, efficiency-oriented thinking, and perseverance in face of challenging problems; Continue absorbing “technical-nutrients” from the development of open-source AI community.

## Skills
- Computer Languages: Rust, Python, C++, Jave, SQL, cypher. 
- Tools for Machine Learning and Deep Learning Models Training and Deployment: Pytorch, Tensorflow, pytorch-lightning, scipy, LightGBM, sklearn, DeepGraphLibrary.)
- Data Engineering Skills:
  1. Experience in Large-scale Analytical Data Service Design, Development, and Maintainance (Airflow, Kibana, FastAPI, Grafana). 
  2. Familiar with Relational and Graph Data Processing Tools (Postgres DB, Duck DB, Neo4j, pandas, polars, and cuDF, PostgresSQL, cypher, Ray). 
- Python tools developement:
  1. Esun in-house python packages for AI operation: sql-tools, [etl-framework](https://coscup.org/2023/zh-TW/session/FHMWYE), avm-tool
  2. Package for ETL: [batch-framework](https://pypi.org/project/batch-framework/)
  3. Rust-based Python package: [JSkiner](https://pypi.org/project/JSkiner/)
  4. LLM-based PyPi package: [regex-inference](https://pypi.org/project/regex-inference/)
  5. Other PyPi packages: [random-regex](https://pypi.org/project/random-regex/), [jsonschema-inference](https://pypi.org/project/jsonschema-inference/)
- Project Management: Scrum, Kanban, Gantt Chart.  


## PROJECT

### Scale-Up Data Pipeline of Graph Data as a Service
**2024/1-2024/12**

**Goal**

1. Refactor a RDB-to-GraphDB data pipeline architecture to enhance its scalability and maintainability. 
2. Reduce the data update latency and increase the data reload throughput. 
3. Enhance the data lineage explainabity for easier data governance. 
4. Enhance the integration testing workflow to facilitate team's code delivery efficiency and quality.

**Responsibility**

- Responsible for planning new architecture components based on the goals set by the manager.
- Assist the manager in translating objectives into development tasks for team members and clarifying task dependencies.
- Conduct code reviews to ensure development quality and manage the integration and conflict resolution of features.

**Accomplishment**

1. Dramatically reduce the data update latency from 2.7 hrs to 1.2 hrs by incorporating incremental update mechanisms, reducing the daily computation and networking of data from 13.5 Gb to 0.5 Mb.
2. Enhance code managability, team agility, and data quality:
   - Across 37 input and 26 output tables and 209 in-between temporary tables.
   - How?
      - Decompose ETL procedures into 5 layers of 450 tasks (I. column-cleaning: 37 x 3 tasks, II. re-mapping: 30 tasks, III. node/link extraction: 179 tasks, IV. node/link aggregation: 26 tasks, and V. neo4j injestion: 26 x 4 tasks).
      - Adopt layer-wise functional testing and between-layer data validation.
3. Apply column-level lineage parsing to all SQLs to support easier identification of the source for each of the graph elements (aka. node, link, and their properties). 
4. Design the day-two operation strategy and implement dashboard and alert mechanism to monitor the pipeline.

### Prototyping and Product Landing of Graph Data Service
**2023/1-2023/12**

**Goal**
1. Prototype a graph datalake to support business units on customer risk-and-value exploration. 

**Responsibility**
1. Collebrate with project manager to conduct user interviews and convert the insight into product blue-print.
2. Lead a product development team of 3 data scientists to conduct raw data exploration and transformation to enrich the graph content.

**Accomplishment**
1. Build from scratch the core of two E.SUN customer insight applications capable of connecting 7 types of enities (people/company/account/ip/device/phone/email) via 15 types of in-between relationships.
2. Setup a Neo4j development environment to speed up the pattern matching of people connections and risky account activities.
3. Build from scratch a RDB-to-GraphDB ETL development framework to ensure the extentability and maintainability of the product.

### Next-Generation ETL Framework for Data Science Team

**2022/7-2022/12**

**Goal:**
1. Design a lightweight ETL python framework enabling data scientists to seamlessly deploy their pandas/SQL processes to airflow in a maintainable format.
2. Reduce the maintenance and optimization cost of AI projects with integration of customizable data validation, metadata registration, and time/memory-profiling tools.
3. Ensure flexibility and extensibility in pandas-like packages (such as CuDF, Polars, PySpark, etc) for future parallelizability, targeting 1000X speedup.

**Responsibility:** Coordinate the design and development of ETL framework components. Give instruction to ETL research intern and provide code review and design guidance for the project participants.

**Accomplishment:** Have wrapped the framework into a workable python package and successfully imported it into two production projects, with ETL business logic automatically rendered on the Airflow UI in an easily traceable way.


### Enhance and Maintain House Price and Mortgage Loan API
**2022/2-2022/7**

**Responsibility:**
API Service maintenance, code refactoring, and model performance enhancement for the house-price/mortgage loan automatic appraisal system.
**Accomplishment:**
1. **Encrypted API re-routing:** Re-route the internal mortgage API service as an encrypted API service for external client. Understand and implement the RSA/AES double encryption protocol under spec-ambiguous situation by investigating client-side PHP code.
2. **Code refactor and migration:** Reduce the cognitive complexity of service code from 1000-line-single-file situation by thoroughly understanding the business logic and refactoring it into chain-of-command design pattern. Design common module with logging mechanism to reduce future maintenance cost. Draw and carry out the code migration plan without compromising the 24/7-criteria.
3. **Re-design of house appraisal model for interpretability:** Coordinate with research institution and business unit to build a business interpretable deep learning model. Re-design the loss function with regularization term to meet the legal requirements. Reducing the model inference time by adopting Google’s state-of-the-art nearest neighbor algorithm for referential house searching.

### Scalable ETL Pipeline for Credit Loan Marketing Data
**2021/8-2022/1**

**Responsibility:**
1. Orchestrate the cross-department coordination of the development process.
2. Design a low-code python-SQL interface for the data-analyst of business unit and provide development and CICD guidance.
3. Ensure business-logic-extensibility in considerations of future marketing campaign.
4. Ensure timely delivery of 7 million customer campaign data under 1day computation criteria.

**Accomplishment:**
1. Have helped the data-analyst of business unit successfully incorporate new campaign business logic into the production pipeline.
2. A comprehensive tutorial to the development interface and CICD toolkits, enabling smooth new feature extension with zero-guidance.
3. Significantly speedup the pipeline from 5d to 8h via map-reduce parallelization with multiple Airflow worker nodes.

### PyTorch development framework for Industry-Academy Cooperation
**2021/4-2022/8**

**Goal:** Develop Pytorch model development framework to reduce the academy-to-company code migration cost.

**Features:**
1. Support training, validation, testing, weight/performance inspection, and check-pointing of models with different architecture.
2. Fixed experimentation flow for all models with formatted running script and folder structure, to enhance code readability and reproducibility.
3. Support lazy evaluation and visualization of data pre-processing, avoid re-generation of data in experimentation scenario.
4. Supporting parallel model hyper-parameter tuning via Ray (a general python parallelization framework).

**Tools:** Pytorch-lightning, Ray, TensorBoard, pyflow-viz

## RESEARCH
### Develop techniques applicable to the music industry and design experiments for proof-of-concept
**2015/9-2020/1**

Instructor: Professor Homer H. Chen

- Developed a context-based tag propagation method to reduce the training noise and successfully improved a deep
music auto-tagging model (SampleCNN) by 25.8% in the MAP.
- Enhance the robustness of the tag propagation method and successfully extended the improvement to two other
neural networks (CRNN and 2D-CNN) with the increase of improvement reaches 6.5%, 4.9%, and 5.5% (for
SampleCNN, CRNN, and 2D-CNN, respectively).

**Responsibility**: 

- Build up the experiment acceleration (via GPU) environment on a Linux-based server; Design the
model evaluation and training strategy with TensorFlow.
- Conduct error analysis to understand the problem in the training data using Matplotlib and Seaborn. Tune the
hyper-parameters during model development. Accelerate the evaluation and data visualization process using ray, a
parallel processing package.

## Education 

### M.S. in Graduate Institude of Communication Engineering, National Taiwan University
**2015/9~2020/1**

- Multimedia Signal Processing (A)
- Computational Methods and Tools for Data Science (A): Familiarize myself with basic EDA techniques. 

### B.S. in Electrical Engineering Department, National Tsing Hua University
**2011/9~2015/6**

- Programming and Hardware Classes: Logic Design (A+) / Logic Design Lab - verilog and FPGA (A+) / Embedding System Lab - C language on Arduino (A+) / Computer Programming Design - C++ (A+)
- Math Classes: Calculus I&II (A+/A+) / Linear Algebra (A+) / Numerical Analysis (A)


