# 2022 Resume

# Jeffrey Lin (林奕勳)

ESUN Bank, Intelligent Finance Technology Department, AI Engineer focusing on Enterprise-Level ML Frameworks and Design Patterns
jeffrey82221@gmail.com TW, Taipei

## CAREER SUMMARY

6+ years of deep learning research and development experience, with a strong ability in prototyping, evaluation, and deployment of models, in both academical and industrial environment.
2+ years of financial AI development experience, specialized in the design of python API, SDK, and framework for optimizing the deployment flow of data science, ETL, and machine learning pipelines.
1+ year of participation in the technology management assistant bootcamp, with real-experience on business user support, gaining first-hand insight on financial and corporative AI usage via cross-department collaboration.
Having excellent code-quality standard, efficiency-oriented thinking, and perseverance in face of challenging problems; Continue absorbing “technical-nutrients” from the development of open-source AI community.

## PROJECT

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
**Responsibility:** API Service maintenance, code refactoring, and model performance enhancement for the house-price/mortgage loan automatic appraisal system.
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

Developed a context-based tag propagation method to reduce the training noise and successfully improved a deep
music auto-tagging model (SampleCNN) by 25.8% in the MAP.
Enhance the robustness of the tag propagation method and successfully extended the improvement to two other
neural networks (CRNN and 2D-CNN) with the increase of improvement reaches 6.5%, 4.9%, and 5.5% (for
SampleCNN, CRNN, and 2D-CNN, respectively).

**Responsibility**: Build up the experiment acceleration (via GPU) environment on a Linux-based server; Design the
model evaluation and training strategy with TensorFlow.
Conduct error analysis to understand the problem in the training data using Matplotlib and Seaborn. Tune the
hyper-parameters during model development. Accelerate the evaluation and data visualization process using ray, a
parallel processing package.

