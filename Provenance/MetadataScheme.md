### OpenDataology metadata 

#### scheme
| field |  describe   | format | range |  is SPDX3 model |
| --- |  ----  | ----  | --- | --- |
| datasetName |  name of dataset   | String | no limit | Y |
| datasetType |  Type describes the datatype contained in the dataset. For example a dataset can be an image dataset for computer vision applications, a text dataset such as the contents of a book or Wikipedia article, or sometimes a multimodal dataset that contains multiple types of data.  | String | DatasetType | Y |
| dataCollectionProcess | DataCollectionProcess describes how a dataset was collected. Examples include the sources from which a dataset was scrapped or the interview protocol that was used for data collection. | String  | no limit | Y |
| intendedUse | IntendedUse describes what the given dataset should be used for. Some datasets are collected to be used only for particular purposes. For example, medical data collected from a specific demography might only be applicable for training machine learning models to make predictions for that demography. In such a case, the intendedUse field would capture this information. Similarly, if a dataset is collected for building a facial recognition model, the intendedUse field would specify that. | String  |no limit| Y |
| datasetSize | DatasetSize Captures how large a dataset is. The size is to be measured in bytes. | number |  nonNegativeInteger （unit Byte） | Y |
| datasetNoise | DatasetNoise describes what kinds of noises a dataset might encompass. The field uses free form text to specify the fields or the samples that might be noisy. Alternatively, it can also be used to describe various noises that could impact the whole dataset. | String | no limit | Y |
| dataPreprocessing | DataPreprocessing describes the various preprocessing steps that were applied to the raw data to create the dataset. | String| no limit | Y |
| sensor | Sensor describes a sensor that was used for collecting the data and its calibration value as a key-value pair. | Map {"key":"value"}  | no limit | Y |
| knownBias | KnownBias is a free form text field that describes the different biases that the dataset encompasses. | String | no limit | Y |
| sensitivePersonalInformation | SensitivePersonalInformation indicates the presence of sensitive personal data or information that allows drawing conclusions about a person's identity. | String | PresenceType | Y |
| anonymizationMethodUsed | AnonymizationMethodUsed describes the methods used to anonymize the dataset (of fields in the dataset). | String | no limit | Y |
| confidentialityLevel | ConfidentialityLevel describes the levels of confidentiality of the data points contained in the dataset.  | String | ConfidentialityLevelType |Y |
| datasetUpdateMechanism | DatasetUpdateMechanism describes a mechanism to update the dataset. | String | no limit | Y |
| datasetAvailability | Some datasets are publicly available and can be downloaded directly. Others are only accessible behind a clickthrough, or after filling a registration form. This field will describe the dataset availability from that perspective. | String | DatasetAvailabilityType | Y |
| version | what is the versioning of the data file used | String | no limit | N |
| originator | who created the dataset | String | no limit | N |
| location | path to directory where input data is stored | String |  no limit  | N |
| concludedLicense | Certified in the SPDX License list and certified by a lawyer | String | no limit | N |
| declaredLicense | Licenses certified in the SPDX License List | String | no limit | N |
| checksum | Calculate the summary of the dataset entities using a specific summary algorithm | CheckSumObject | no limit | N |
| offensiveContent | Does it include explicit descriptions or photos | String | PresenceType  | N |
| assembledDate | The date obtained from the composition of data in a dataset | Date | "YYYY-MM-DD mm:ss" | N |
| obtainedDate | Date when the dataset entered the data warehouse | Date | "YYYY-MM-DD mm:ss" | N |
| releaseDate | Date of dataset release version | Date | "YYYY-MM-DD mm:ss" | N |
| validUntilDate | License specifies the effective date of the dataset | Date | "YYYY-MM-DD mm:ss" | N |
| standards | What data standards are followed for the content in the dataset. | Date | "YYYY-MM-DD mm:ss" | N |
| errata | Specific text describing incorrect aspects of the dataset. | String | no limit|N |
| datasetSupplier | Individuals or organizations providing datasets | String | no limit | N |

#### Datatype
* [DatasetType](https://github.com/spdx/spdx-3-model/blob/fc9f50625a99b82c2f24b18f175f52f6b7d46e10/model/Dataset/Vocabularies/DatasetType.md#L4)
* [PresenceType](https://github.com/spdx/spdx-3-model/blob/fc9f50625a99b82c2f24b18f175f52f6b7d46e10/model/AI/Vocabularies/PresenceType.md#L4)
* [ConfidentialityLevelType](https://github.com/spdx/spdx-3-model/blob/fc9f50625a99b82c2f24b18f175f52f6b7d46e10/model/Dataset/Vocabularies/ConfidentialityLevelType.md#L4)
* [DatasetAvailabilityType](https://github.com/spdx/spdx-3-model/blob/fc9f50625a99b82c2f24b18f175f52f6b7d46e10/model/Dataset/Vocabularies/DatasetAvailabilityType.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          