<!---
   Copyright 2017-2022 Ericsson AB.
   For a full list of individual contributors, please see the commit history.

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
--->

# Eiffel Protocol in PMeta
PMeta框架采用了开源的Eiffel Protocol, 该协议是不依赖具体实现技术的CI/CD消息协议。

本代码仓包含了Eiffel协议的词汇, 详细描述, 结构定义和设计指南。

PMeta的参考架构设计，请参见 [PMeta的设计文档](./PMeta%E8%AE%BE%E8%AE%A1%E6%96%87%E6%A1%A3.pdf)


# Contents
1. Introduction
   1. [Introduction](./introduction/introduction.md)
   1. [How to Propose Changes and Contribute](https://github.com/eiffel-community/.github/blob/master/CONTRIBUTING.md)
   1. [Code of Conduct](https://github.com/eiffel-community/.github/blob/master/CODE_OF_CONDUCT.md)
1. Eiffel Syntax and Usage
   1. [Eiffel Glossary](./eiffel-syntax-and-usage/glossary.md)
   1. [Event Design Guidelines](./eiffel-syntax-and-usage/event-design-guidelines.md)
   1. [Event Structure](./eiffel-syntax-and-usage/event-structure.md)
   1. [The Meta Object](./eiffel-syntax-and-usage/the-meta-object.md)
   1. [The Links Object](./eiffel-syntax-and-usage/the-links-object.md)
   1. [Versioning](./eiffel-syntax-and-usage/versioning.md)
   1. [Compositions and Validity Checking](./eiffel-syntax-and-usage/compositions-and-validity-checking.md)
   1. [Security](./eiffel-syntax-and-usage/security.md)
   1. [Activity Linking](./eiffel-syntax-and-usage/activity-linking.md)
   1. [Event Schemas](./eiffel-syntax-and-usage/event-schemas.md)
   1. [Event Categories](./eiffel-syntax-and-usage/event-categories.md)
1. The Eiffel Vocabulary
   1. [EiffelActivityTriggeredEvent (ActT)](./eiffel-vocabulary/EiffelActivityTriggeredEvent.md)
   1. [EiffelActivityCanceledEvent (ActC)](./eiffel-vocabulary/EiffelActivityCanceledEvent.md)
   1. [EiffelActivityStartedEvent (ActS)](./eiffel-vocabulary/EiffelActivityStartedEvent.md)
   1. [EiffelActivityFinishedEvent (ActF)](./eiffel-vocabulary/EiffelActivityFinishedEvent.md)
   1. [EiffelArtifactCreatedEvent (ArtC)](./eiffel-vocabulary/EiffelArtifactCreatedEvent.md)
   1. [EiffelArtifactPublishedEvent (ArtP)](./eiffel-vocabulary/EiffelArtifactPublishedEvent.md)
   1. [EiffelArtifactReusedEvent (ArtR)](./eiffel-vocabulary/EiffelArtifactReusedEvent.md)
   1. [EiffelConfidenceLevelModifiedEvent (CLM)](./eiffel-vocabulary/EiffelConfidenceLevelModifiedEvent.md)
   1. [EiffelEnvironmentDefinedEvent (ED)](./eiffel-vocabulary/EiffelEnvironmentDefinedEvent.md)
   1. [EiffelCompositionDefinedEvent (CD)](./eiffel-vocabulary/EiffelCompositionDefinedEvent.md)
   1. [EiffelSourceChangeCreatedEvent (SCC)](./eiffel-vocabulary/EiffelSourceChangeCreatedEvent.md)
   1. [EiffelSourceChangeSubmittedEvent (SCS)](./eiffel-vocabulary/EiffelSourceChangeSubmittedEvent.md)
   1. [EiffelFlowContextDefinedEvent (FCD)](./eiffel-vocabulary/EiffelFlowContextDefinedEvent.md)
   1. [EiffelTestCaseTriggeredEvent (TCT)](./eiffel-vocabulary/EiffelTestCaseTriggeredEvent.md)
   1. [EiffelTestCaseCanceledEvent (TCC)](./eiffel-vocabulary/EiffelTestCaseCanceledEvent.md)
   1. [EiffelTestCaseStartedEvent (TCS)](./eiffel-vocabulary/EiffelTestCaseStartedEvent.md)
   1. [EiffelTestCaseFinishedEvent (TCF)](./eiffel-vocabulary/EiffelTestCaseFinishedEvent.md)
   1. [EiffelTestSuiteStartedEvent (TSS)](./eiffel-vocabulary/EiffelTestSuiteStartedEvent.md)
   1. [EiffelTestSuiteFinishedEvent (TSF)](./eiffel-vocabulary/EiffelTestSuiteFinishedEvent.md)
   1. [EiffelIssueVerifiedEvent (IV)](./eiffel-vocabulary/EiffelIssueVerifiedEvent.md)
   1. [EiffelTestExecutionRecipeCollectionCreatedEvent (TERCC)](./eiffel-vocabulary/EiffelTestExecutionRecipeCollectionCreatedEvent.md)
   1. [EiffelAnnouncementPublishedEvent (AnnP)](./eiffel-vocabulary/EiffelAnnouncementPublishedEvent.md)
   1. [EiffelIssueDefinedEvent (ID)](./eiffel-vocabulary/EiffelIssueDefinedEvent.md)
1. Usage Examples
   1. [Confidence Level Joining](./usage-examples/confidence-level-joining.md)
   1. [Delivery Interface](./usage-examples/delivery-interface.md)
   1. [Build Avoidance](./usage-examples/build-avoidance.md)
   1. [Pipeline Monitoring](./usage-examples/pipeline-monitoring.md)
   1. [Test Execution](./usage-examples/test-execution.md)
   1. Reference Data Sets
      1. [Default](./usage-examples/reference-data-sets/default.md)
1. Customization
   1. [Custom Events](./customization/custom-events.md)
   1. [Custom Data](./customization/custom-data.md)
1. Extensions
   1. [Eiffel Operations Extension](https://github.com/Ericsson/eiffel-operations-extension)
