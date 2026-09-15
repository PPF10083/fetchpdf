# 多领域文献全文获取测试数据集

核验时间（UTC）：2026-09-12T02:51:40.2017530Z。共 100 篇，OA / 非 OA 各 50 篇，True 在前、False 在后；每类内按领域排列。

判定口径：OpenAlex 文章级 open_access.is_oa；True 选取 gold/hybrid 且出版社主位置开放的文章，False 要求 oa_status=closed。DOI、标题与期刊名称逐篇通过 Crossref 核对，URL 优先使用 Crossref 登记的出版社落地页，缺失时使用 DOI 链接。来源列为期刊名称。

注意：这是检索时元数据快照，不是对实时全文访问、授权许可或绝对不存在开放副本的保证；未逐篇测试下载。非 OA 不等于 DOI 或摘要页无法访问，网页访问失败也不等于非 OA。样本按领域内引用量优先选取并限制期刊重复，不是随机或代表性统计样本。

| 是否 OA | DOI | 标题 | URL | 来源 |
| ----- | ----- | ----- | ----- | ----- |
| True | 10.3322/caac.21660 | Global Cancer Statistics 2020: GLOBOCAN Estimates of Incidence and Mortality Worldwide for 36 Cancers in 185 Countries | https://acsjournals.onlinelibrary.wiley.com/doi/10.3322/caac.21660 | CA: A Cancer Journal for Clinicians |
| True | 10.1038/s41586-020-2012-7 | A pneumonia outbreak associated with a new coronavirus of probable bat origin | https://www.nature.com/articles/s41586-020-2012-7 | Nature |
| True | 10.1016/s0140-6736(20)30925-9 | Global burden of 369 diseases and injuries in 204 countries and territories, 1990–2019: a systematic analysis for the Global Burden of Disease Study 2019 | https://linkinghub.elsevier.com/retrieve/pii/S0140673620309259 | The Lancet |
| True | 10.1136/bjsports-2020-102955 | World Health Organization 2020 guidelines on physical activity and sedentary behaviour | https://bjsm.bmj.com/lookup/doi/10.1136/bjsports-2020-102955 | British Journal of Sports Medicine |
| True | 10.1016/j.jacc.2020.11.010 | Global Burden of Cardiovascular Diseases and Risk Factors, 1990–2019 | https://linkinghub.elsevier.com/retrieve/pii/S0735109720377755 | Journal of the American College of Cardiology |
| True | 10.1038/s41586-021-03819-2 | Highly accurate protein structure prediction with AlphaFold | https://www.nature.com/articles/s41586-021-03819-2 | Nature |
| True | 10.1093/molbev/msab120 | MEGA11: Molecular Evolutionary Genetics Analysis Version 11 | https://academic.oup.com/mbe/article/38/7/3022/6248099 | Molecular Biology and Evolution |
| True | 10.1093/gigascience/giab008 | Twelve years of SAMtools and BCFtools | https://academic.oup.com/gigascience/article/doi/10.1093/gigascience/giab008/6137722 | GigaScience |
| True | 10.1016/j.cell.2021.04.048 | Integrated analysis of multimodal single-cell data | https://linkinghub.elsevier.com/retrieve/pii/S0092867421005833 | Cell |
| True | 10.1016/j.xinn.2021.100141 | clusterProfiler 4.0: A universal enrichment tool for interpreting omics data | https://linkinghub.elsevier.com/retrieve/pii/S2666675821000667 | The Innovation |
| True | 10.1038/s41592-019-0686-2 | SciPy 1.0: fundamental algorithms for scientific computing in Python | https://www.nature.com/articles/s41592-019-0686-2 | Nature Methods |
| True | 10.1186/s40537-021-00444-8 | Review of deep learning: concepts, CNN architectures, challenges, applications, future directions | https://journalofbigdata.springeropen.com/articles/10.1186/s40537-021-00444-8 | Journal of Big Data |
| True | 10.1145/3503250 | NeRF | https://dl.acm.org/doi/10.1145/3503250 | Communications of the ACM |
| True | 10.1186/s12864-019-6413-7 | The advantages of the Matthews correlation coefficient (MCC) over F1 score and accuracy in binary classification evaluation | https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-019-6413-7 | BMC Genomics |
| True | 10.1016/j.aiopen.2021.01.001 | Graph neural networks: A review of methods and applications | https://linkinghub.elsevier.com/retrieve/pii/S2666651021000012 | AI Open |
| True | 10.1109/jsac.2022.3156632 | Integrated Sensing and Communications: Toward Dual-Functional Wireless Networks for 6G and Beyond | https://ieeexplore.ieee.org/document/9737357/ | IEEE Journal on Selected Areas in Communications |
| True | 10.1038/s41467-019-14108-y | The role of artificial intelligence in achieving the Sustainable Development Goals | https://www.nature.com/articles/s41467-019-14108-y | Nature Communications |
| True | 10.1007/s11157-020-09523-3 | Biochar physicochemical properties: pyrolysis temperature and feedstock kind effects | http://link.springer.com/10.1007/s11157-020-09523-3 | Reviews in Environmental Science and Bio/Technology |
| True | 10.1109/access.2020.2998358 | Digital Twin: Enabling Technologies, Challenges and Open Research | https://ieeexplore.ieee.org/document/9103025/ | IEEE Access |
| True | 10.1016/j.jmsy.2021.10.006 | Industry 4.0 and Industry 5.0—Inception, conception and perception | https://linkinghub.elsevier.com/retrieve/pii/S0278612521002119 | Journal of Manufacturing Systems |
| True | 10.1063/5.0004608 | The ORCA quantum chemistry program package | https://pubs.aip.org/jcp/article/152/22/224108/1061982/The-ORCA-quantum-chemistry-program-package | The Journal of Chemical Physics |
| True | 10.1107/s1600576721002910 | CrystalExplorer : a program for Hirshfeld surface analysis, visualization and quantitative analysis of molecular crystals | https://journals.iucr.org/paper?S1600576721002910 | Journal of Applied Crystallography |
| True | 10.1016/j.jqsrt.2021.107949 | The HITRAN2020 molecular spectroscopic database | https://linkinghub.elsevier.com/retrieve/pii/S0022407321004416 | Journal of Quantitative Spectroscopy and Radiative Transfer |
| True | 10.1038/s41598-021-99269-x | Management of validation of HPLC method for determination of acetylsalicylic acid impurities in a new pharmaceutical product | https://www.nature.com/articles/s41598-021-99269-x | Scientific Reports |
| True | 10.3390/ijms22073380 | Analytical Methods Used in Determining Antioxidant Activity: A Review | https://www.mdpi.com/1422-0067/22/7/3380 | International Journal of Molecular Sciences |
| True | 10.1093/ptep/ptac097 | Review of Particle Physics | https://academic.oup.com/ptep/article/doi/10.1093/ptep/ptac097/6651666 | Progress of Theoretical and Experimental Physics |
| True | 10.1063/5.0007045 | CP2K: An electronic structure and molecular dynamics software package - Quickstep: Efficient and accurate electronic structure calculations | https://pubs.aip.org/jcp/article/152/19/194103/199081/CP2K-An-electronic-structure-and-molecular | The Journal of Chemical Physics |
| True | 10.1051/0004-6361/202243940 | Gaia Data Release 3 | https://www.aanda.org/10.1051/0004-6361/202243940 | Astronomy & Astrophysics |
| True | 10.1103/physrevd.110.030001 | Review of Particle Physics | https://link.aps.org/doi/10.1103/PhysRevD.110.030001 | Physical Review D |
| True | 10.1007/s10915-022-01939-z | Scientific Machine Learning Through Physics–Informed Neural Networks: Where we are and What’s Next | https://link.springer.com/10.1007/s10915-022-01939-z | Journal of Scientific Computing |
| True | 10.1017/rdc.2020.41 | The IntCal20 Northern Hemisphere Radiocarbon Age Calibration Curve (0–55 cal kBP) | https://www.cambridge.org/core/product/identifier/S0033822220000417/type/journal_article | Radiocarbon |
| True | 10.1038/s41467-020-20314-w | Anomalous collapses of Nares Strait ice arches leads to enhanced export of Arctic sea ice | https://www.nature.com/articles/s41467-020-20314-w | Nature Communications |
| True | 10.5194/essd-13-4349-2021 | ERA5-Land: a state-of-the-art global reanalysis dataset for land applications | https://essd.copernicus.org/articles/13/4349/2021/ | Earth System Science Data |
| True | 10.1029/2019jb018774 | Present‐Day Crustal Deformation of Continental China Derived From GPS and Its Tectonic Implications | https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019JB018774 | Journal of Geophysical Research: Solid Earth |
| True | 10.1126/sciadv.aaz1346 | Cenozoic sea-level and cryospheric evolution from deep-sea geochemical and continental margin records | https://www.science.org/doi/10.1126/sciadv.aaz1346 | Science Advances |
| True | 10.1002/qj.3803 | The ERA5 global reanalysis | https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.3803 | Quarterly Journal of the Royal Meteorological Society |
| True | 10.1016/s0140-6736(20)30752-2 | Global burden of 87 risk factors in 204 countries and territories, 1990–2019: a systematic analysis for the Global Burden of Disease Study 2019 | https://linkinghub.elsevier.com/retrieve/pii/S0140673620307522 | The Lancet |
| True | 10.3389/fpubh.2020.00014 | Environmental and Health Impacts of Air Pollution: A Review | https://www.frontiersin.org/article/10.3389/fpubh.2020.00014/full | Frontiers in Public Health |
| True | 10.1016/j.heliyon.2020.e04691 | Heavy metal pollution in the environment and their toxicological effects on humans | https://linkinghub.elsevier.com/retrieve/pii/S2405844020315346 | Heliyon |
| True | 10.1021/acs.analchem.0c01887 | AGREE─Analytical GREEnness Metric Approach and Software | https://pubs.acs.org/ancham/article/92/14/10076/826812/AGREE-Analytical-GREEnness-Metric-Approach-and | Analytical Chemistry |
| True | 10.1038/s41562-021-01079-8 | A global panel database of pandemic policies (Oxford COVID-19 Government Response Tracker) | https://www.nature.com/articles/s41562-021-01079-8 | Nature Human Behaviour |
| True | 10.1080/09669582.2020.1758708 | Pandemics, tourism and global change: a rapid assessment of COVID-19 | https://www.tandfonline.com/doi/full/10.1080/09669582.2020.1758708 | Journal of Sustainable Tourism |
| True | 10.1093/rfs/hhaa009 | Empirical Asset Pricing via Machine Learning | https://academic.oup.com/rfs/article/33/5/2223/5758276 | The Review of Financial Studies |
| True | 10.1093/qje/qjaa004 | The Fall of the Labor Share and the Rise of Superstar Firms* | https://academic.oup.com/qje/article/135/2/645/5721266 | The Quarterly Journal of Economics |
| True | 10.1016/j.jfineco.2020.11.001 | Responsible investing: The ESG-efficient frontier | https://linkinghub.elsevier.com/retrieve/pii/S0304405X20302853 | Journal of Financial Economics |
| True | 10.3390/ijerph17051729 | Immediate Psychological Responses and Associated Factors during the Initial Stage of the 2019 Coronavirus Disease (COVID-19) Epidemic among the General Population in China | https://www.mdpi.com/1660-4601/17/5/1729 | International Journal of Environmental Research and Public Health |
| True | 10.1001/jamanetworkopen.2020.3976 | Factors Associated With Mental Health Outcomes Among Health Care Workers Exposed to Coronavirus Disease 2019 | https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2763229 | JAMA Network Open |
| True | 10.1016/s2215-0366(21)00395-3 | Global, regional, and national burden of 12 mental disorders in 204 countries and territories, 1990–2019: a systematic analysis for the Global Burden of Disease Study 2019 | https://linkinghub.elsevier.com/retrieve/pii/S2215036621003953 | The Lancet Psychiatry |
| True | 10.1177/0047239520934018 | Online Learning: A Panacea in the Time of COVID-19 Crisis | https://journals.sagepub.com/doi/10.1177/0047239520934018 | Journal of Educational Technology Systems |
| True | 10.1007/s11469-020-00270-8 | The Fear of COVID-19 Scale: Development and Initial Validation | https://link.springer.com/10.1007/s11469-020-00270-8 | International Journal of Mental Health and Addiction |
| False | 10.1016/j.jamda.2019.12.012 | Asian Working Group for Sarcopenia: 2019 Consensus Update on Sarcopenia Diagnosis and Treatment | https://linkinghub.elsevier.com/retrieve/pii/S1525861019308722 | Journal of the American Medical Directors Association |
| False | 10.1001/jama.2020.4683 | Case-Fatality Rate and Characteristics of Patients Dying in Relation to COVID-19 in Italy | https://jamanetwork.com/journals/jama/fullarticle/2763667 | JAMA |
| False | 10.1038/s41591-023-02448-8 | Large language models in medicine | https://www.nature.com/articles/s41591-023-02448-8 | Nature Medicine |
| False | 10.1093/cvr/cvac013 | Global burden of heart failure: a comprehensive and updated review of epidemiology | https://academic.oup.com/cardiovascres/article/118/17/3272/6527627 | Cardiovascular Research |
| False | 10.2337/dc21-s002 | 2. Classification and Diagnosis of Diabetes: Standards of Medical Care in Diabetes—2021 | https://diabetesjournals.org/care/article/44/Supplement_1/S15/30859/2-Classification-and-Diagnosis-of-Diabetes | Diabetes Care |
| False | 10.1016/j.cell.2022.11.001 | Hallmarks of aging: An expanding universe | https://linkinghub.elsevier.com/retrieve/pii/S0092867422013770 | Cell |
| False | 10.1038/s41592-020-01018-x | Cellpose: a generalist algorithm for cellular segmentation | https://www.nature.com/articles/s41592-020-01018-x | Nature Methods |
| False | 10.1016/j.molp.2023.09.010 | TBtools-II: A “one for all, all for one” bioinformatics platform for biological big-data mining | https://linkinghub.elsevier.com/retrieve/pii/S1674205223002812 | Molecular Plant |
| False | 10.1038/s41596-020-0292-x | CellPhoneDB: inferring cell–cell communication from combined expression of multi-subunit ligand–receptor complexes | https://www.nature.com/articles/s41596-020-0292-x | Nature Protocols |
| False | 10.1002/cpbi.102 | Using SPAdes De Novo Assembler | https://currentprotocols.onlinelibrary.wiley.com/doi/10.1002/cpbi.102 | Current Protocols in Bioinformatics |
| False | 10.1109/jproc.2020.3004555 | A Comprehensive Survey on Transfer Learning | https://ieeexplore.ieee.org/document/9134370/ | Proceedings of the IEEE |
| False | 10.1109/tpami.2020.2983686 | Deep High-Resolution Representation Learning for Visual Recognition | https://ieeexplore.ieee.org/document/9052469/ | IEEE Transactions on Pattern Analysis and Machine Intelligence |
| False | 10.1016/j.neucom.2021.03.091 | A review on the attention mechanism of deep learning | https://linkinghub.elsevier.com/retrieve/pii/S092523122100477X | Neurocomputing |
| False | 10.1109/tip.2021.3051462 | EnlightenGAN: Deep Light Enhancement Without Paired Supervision | https://ieeexplore.ieee.org/document/9334429/ | IEEE Transactions on Image Processing |
| False | 10.1109/comst.2020.2986024 | Federated Learning in Mobile Edge Networks: A Comprehensive Survey | https://ieeexplore.ieee.org/document/9060868/ | IEEE Communications Surveys & Tutorials |
| False | 10.1016/j.scib.2020.01.001 | 18% Efficiency organic solar cells | https://linkinghub.elsevier.com/retrieve/pii/S2095927320300013 | Science Bulletin |
| False | 10.1109/tpami.2020.3005434 | Deep Learning for 3D Point Clouds: A Survey | https://ieeexplore.ieee.org/document/9127813/ | IEEE Transactions on Pattern Analysis and Machine Intelligence |
| False | 10.1016/j.joule.2022.05.005 | The timescale identification decoupling complicated kinetic processes in lithium batteries | https://linkinghub.elsevier.com/retrieve/pii/S254243512200232X | Joule |
| False | 10.1038/s41565-020-0655-z | Memory devices and applications for in-memory computing | https://www.nature.com/articles/s41565-020-0655-z | Nature Nanotechnology |
| False | 10.1002/adma.201908205 | Single‐Junction Organic Photovoltaic Cells with Approaching 18% Efficiency | https://advanced.onlinelibrary.wiley.com/doi/10.1002/adma.201908205 | Advanced Materials |
| False | 10.1002/jcc.26812 | Independent gradient model based on Hirshfeld partition: A new method for visual study of interactions in chemical systems | https://onlinelibrary.wiley.com/doi/10.1002/jcc.26812 | Journal of Computational Chemistry |
| False | 10.1039/d1cp02805g | Efficient evaluation of electrostatic potential with computerized optimized code | https://pubs.rsc.org/cp/article/23/36/20323-20328/721751 | Physical Chemistry Chemical Physics |
| False | 10.1007/s00204-020-02689-3 | Antioxidants and antioxidant methods: an updated overview | http://link.springer.com/10.1007/s00204-020-02689-3 | Archives of Toxicology |
| False | 10.1016/j.carbon.2020.05.023 | An sp-hybridized all-carboatomic ring, cyclo[18]carbon: Electronic structure, electronic spectrum, and optical nonlinearity | https://linkinghub.elsevier.com/retrieve/pii/S0008622320304644 | Carbon |
| False | 10.1021/acs.jctc.1c00302 | OPLS4: Improving Force Field Accuracy on Challenging Regimes of Chemical Space | https://pubs.acs.org/doi/10.1021/acs.jctc.1c00302 | Journal of Chemical Theory and Computation |
| False | 10.1021/acs.jctc.1c00645 | gmx_MMPBSA: A New Tool to Perform End-State Free Energy Calculations with GROMACS | https://pubs.acs.org/doi/10.1021/acs.jctc.1c00645 | Journal of Chemical Theory and Computation |
| False | 10.1137/20m1318043 | Understanding and Mitigating Gradient Flow Pathologies in Physics-Informed Neural Networks | https://epubs.siam.org/doi/10.1137/20M1318043 | SIAM Journal on Scientific Computing |
| False | 10.1038/s41566-021-00780-4 | Structured light | https://www.nature.com/articles/s41566-021-00780-4 | Nature Photonics |
| False | 10.1016/j.comptc.2021.113249 | Shermo: A general code for calculating molecular thermochemistry properties | https://linkinghub.elsevier.com/retrieve/pii/S2210271X21001080 | Computational and Theoretical Chemistry |
| False | 10.1016/j.cma.2021.113741 | A physics-informed deep learning framework for inversion and surrogate modeling in solid mechanics | https://linkinghub.elsevier.com/retrieve/pii/S0045782521000773 | Computer Methods in Applied Mechanics and Engineering |
| False | 10.1016/j.scitotenv.2024.173359 | Greenhouse gases emissions and global climate change: Examining the influence of CO2, CH4, and N2O | https://linkinghub.elsevier.com/retrieve/pii/S004896972403506X | Science of The Total Environment |
| False | 10.1038/s41561-019-0526-0 | Carbon release through abrupt permafrost thaw | https://www.nature.com/articles/s41561-019-0526-0 | Nature Geoscience |
| False | 10.1016/j.earscirev.2021.103503 | Phanerozoic paleotemperatures: The earth’s changing climate during the last 540 million years | https://linkinghub.elsevier.com/retrieve/pii/S0012825221000027 | Earth-Science Reviews |
| False | 10.1038/s41558-020-0855-4 | Rapid worldwide growth of glacial lakes since 1990 | https://www.nature.com/articles/s41558-020-0855-4 | Nature Climate Change |
| False | 10.1098/rsta.2020.0093 | Physics-informed machine learning: case studies for weather and climate modelling | https://royalsocietypublishing.org/doi/10.1098/rsta.2020.0093 | Philosophical Transactions of the Royal Society A: Mathematical, Physical and Engineering Sciences |
| False | 10.1016/j.jhazmat.2020.122383 | Guidelines for the use and interpretation of adsorption isotherm models: A review | https://linkinghub.elsevier.com/retrieve/pii/S030438942030371X | Journal of Hazardous Materials |
| False | 10.1038/s43016-021-00225-9 | Food systems are responsible for a third of global anthropogenic GHG emissions | https://www.nature.com/articles/s43016-021-00225-9 | Nature Food |
| False | 10.1126/science.abg5433 | The global threat from plastic pollution | https://www.science.org/doi/10.1126/science.abg5433 | Science |
| False | 10.1016/j.chemosphere.2020.127279 | Adsorption isotherm models: Classification, physical meaning, application and solving method | https://linkinghub.elsevier.com/retrieve/pii/S0045653520314727 | Chemosphere |
| False | 10.1016/j.ref.2024.100545 | The renewable energy role in the global energy Transformations | https://linkinghub.elsevier.com/retrieve/pii/S1755008424000097 | Renewable Energy Focus |
| False | 10.1257/aer.20191823 | Measuring Geopolitical Risk | https://pubs.aeaweb.org/doi/10.1257/aer.20191823 | American Economic Review |
| False | 10.1007/s00181-020-01875-7 | General diagnostic tests for cross-sectional dependence in panels | https://link.springer.com/10.1007/s00181-020-01875-7 | Empirical Economics |
| False | 10.1016/j.jfineco.2021.01.010 | Corporate green bonds | https://linkinghub.elsevier.com/retrieve/pii/S0304405X21000337 | Journal of Financial Economics |
| False | 10.1016/j.resconrec.2021.105959 | Challenges toward carbon neutrality in China: Strategies and countermeasures | https://linkinghub.elsevier.com/retrieve/pii/S0921344921005681 | Resources, Conservation and Recycling |
| False | 10.1016/j.enpol.2021.112255 | Demand for green finance: Resolving financing constraints on green innovation in China | https://linkinghub.elsevier.com/retrieve/pii/S0301421521001245 | Energy Policy |
| False | 10.1016/j.cedpsych.2020.101860 | Intrinsic and extrinsic motivation from a self-determination theory perspective: Definitions, theory, practices, and future directions | https://linkinghub.elsevier.com/retrieve/pii/S0361476X20300254 | Contemporary Educational Psychology |
| False | 10.1056/nejmp2008017 | Mental Health and the Covid-19 Pandemic | http://www.nejm.org/doi/10.1056/NEJMp2008017 | New England Journal of Medicine |
| False | 10.1002/hbe2.195 | The theory of planned behavior: Frequently asked questions | https://onlinelibrary.wiley.com/doi/10.1002/hbe2.195 | Human Behavior and Emerging Technologies |
| False | 10.1037/amp0000660 | Risk and resilience in family well-being during the COVID-19 pandemic. | https://doi.apa.org/doi/10.1037/amp0000660 | American Psychologist |
| False | 10.1001/jamainternmed.2020.1562 | The Mental Health Consequences of COVID-19 and Physical Distancing | https://jamanetwork.com/journals/jamainternalmedicine/fullarticle/2764404 | JAMA Internal Medicine |

## 领域覆盖

- 医学：OA 5 篇，非 OA 5 篇。
- 生物化学、遗传学与分子生物学：OA 5 篇，非 OA 5 篇。
- 计算机科学：OA 5 篇，非 OA 5 篇。
- 工程学：OA 5 篇，非 OA 5 篇。
- 化学：OA 5 篇，非 OA 5 篇。
- 物理与天文学：OA 5 篇，非 OA 5 篇。
- 地球与行星科学：OA 5 篇，非 OA 5 篇。
- 环境科学：OA 5 篇，非 OA 5 篇。
- 经济、计量经济与金融：OA 5 篇，非 OA 5 篇。
- 心理学：OA 5 篇，非 OA 5 篇。

逐篇领域、OpenAlex OA 字段、检索请求及 Crossref 响应见 `../rd_runs/fulltextfetch/oa-balanced-100/selected.json` 和同目录 JSON 文件。
