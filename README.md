# Breast_Cancer_Classfication
Machine Learning Project 

## Data Description
Source linke: https://ieee-dataport.org/open-access/seer-breast-cancer-data

### Abstract
This dataset of breast cancer patients was obtained from the 2017 November update of the SEER program of the NCI. It provides information on population-based cancer statistics. This data set includes female patients diagonolized with infiltrating duct and lobular carcinoma breast cancer from 2006 to 2010. Patients with unknown tumor size, examined regional LNs, regional positive LNs, and patients whose survival months were less than 1 month were excluded; thus, 4024 patients were ultimately included.

### Features
__1. Age__: numerical, int. The age of the patient at diagnosis for the cancer.

__2. Race__: Nominal Categorical. (White, Black, others). Note that these categorical is unbalanced, with majority being white. This may lead to bias model.

__3. Marital Status__: Nominal Categorical. (Married, Divorced, Single, Widowed, Separated). The patient's marital status at the time of dignosis.

__4. T Stage__: Ordinal Categorical. (T1, T2, T3, T4). T categories for breast cancer. Higher T numbers mean a larger tumor and/or wider spread to tissues near the breast, therefore it is an ordinal categorical feature.

* T1: Tumor is 2 cm (3/4 of an inch) or less across.
* T2: Tumor is more than 2 cm but not more than 5 cm (2 inches) across.
* T3: Tumor is more than 5 cm across.
* T4: Tumor of any size growing into the chest wall or skin. This includes inflammatory breast cancer.

reference: https://www.cancer.org/cancer/breast-cancer/understanding-a-breast-cancer-diagnosis/stages-of-breast-cancer.html

__5. N Stage__: Ordinal Categorical. (N1, N2, N3). N categories for breast cancer. It indicates whether the cancer has spread to lymph nodes near the breast and, if so, how many lymph nodes are involved. It measures how large the cancer is spreaded. A higher value means the cancer is more spreaded, therefore it is an ordinal categorical feature.

* N1: Cancer has spread to 1 to 3 axillary (underarm) lymph node(s), and/or cancer is found in internal mammary lymph nodes (those near the breast bone) on sentinel lymph node biopsy.
* N2: Cancer has spread to 4 to 9 lymph nodes under the arm, or cancer has enlarged the internal mammary lymph nodes
* N3: Any of the following scenario: 1. Cancer has spread to 10 or more axillary lymph nodes, with at least one area of cancer spread greater than 2 mm. 2. Cancer has spread to the lymph nodes under the collarbone (infraclavicular nodes), with at least one area of cancer spread greater than 2 mm. 3. Cancer is found in at least one axillary lymph node (with at least one area of cancer spread greater than 2 mm) and has enlarged the internal mammary lymph nodes. 4. Cancer has spread to 4 or more axillary lymph nodes (with at least one area of cancer spread greater than 2 mm), and to the internal mammary lymph nodes on sentinel lymph node biopsy. 5. Cancer has spread to the lymph nodes above the collarbone (supraclavicular nodes) on the same side of the cancer with at least one area of cancer spread greater than 2 mm.

reference: https://www.cancer.org/cancer/breast-cancer/understanding-a-breast-cancer-diagnosis/stages-of-breast-cancer.html

__6. 6th Stage__: Ordinal Categorical. ('IIIC', 'IIIA', 'IIB', 'IIA', 'IIIB') Created from merged EOD 3rd Edition and Collaborative Stage disease information. It measures the extent of desease. Higher the value (to the left in the above parentasis), the more serious the desease is, therefore it is an ordinal categorical feature. Reference: http://seer.cancer.gov/seerstat/variables/seer/ajcc-stage/6th

__7. Grade__: Ordinal Categorical. (Well differentiated; Grade I, Moderately differentiated; Grade II, Poorly differentiated; Grade III, Undifferentiated; anaplastic; Grade IV). It measures how the tumor is differentiated from its surrounding tissues. Higher the grade is, the less differentiated the tumor is, therefore it is an ordinal categorical feature.

__8. A Stage__: Binary Categorical. (Regional, Distant). 
* Regional: A neoplasm that has extended 1) beyond the limits of the organ of origin
directly into surrounding organs or tissues; 2) into regional lymph nodes by way of the
lymphatic system; or 3) by a combination of extension and regional lymph nodes.
* Distant: Distant — A neoplasm that has spread to parts of the body remote from the primary
tumor either by direct extension or by discontinuous metastasis (e.g., implantation or
seeding) to distant organs, issues, or via the lymphatic system to distant lymph nodes.
Reference: http://seer.cancer.gov/seerstat/variables/seer/lrd-stage

__9. Tumor Size__: Numerical, int. Each indicates exact size in millimeters.

__10. Estrogen Status__: Binary categorical. (positive, negative)
* positive: Breast cancers that have estrogen receptors are called ER-positive (or ER+) cancers.

__11. Progesterone Status__: Binary categorical. (positive, negative)
* positive: Breast cancers with progesterone receptors are called PR-positive (or PR+) cancers.

Note: Breast cancer cells taken out during a biopsy or surgery will be tested to see if they have certain proteins that are estrogen or progesterone receptors. When the hormones estrogen and progesterone attach to these receptors, they stimulate the cancer to grow. Cancers are called hormone receptor-positive or hormone receptor-negative based on whether or not they have these receptors (proteins). reference: https://www.cancer.org/cancer/breast-cancer/understanding-a-breast-cancer-diagnosis/breast-cancer-hormone-receptor-status.html

__12. Regional Node Examined__: Numerical, int. Records the total number of regional lymph nodes that were removed and examined by the pathologist.

__13. Reginol Node Positive__: Numerical, int. : Records the exact number of regional lymph nodes examined by the pathologist that were found to contain metastases.

__14. Survival Months__: Numerical, int. The estimated length of survival (in months). 

__15. Status__: Binary Categorical (response). Dead or Alive.