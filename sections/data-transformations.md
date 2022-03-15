## Amazon SageMaker Data Wrangler

To better understand SageMaker Data Wrangler, it helps to first understand Amazon SageMaker. Data Wranger is a feature of SageMaker so let’s first see how Data Wrangler fits within the broader SageMaker platform.

### What is Amazon SageMaker? 

Amazon SageMaker provides every developer and data scientist with the ability to build, train, and deploy ML models quickly and at lower cost by providing the tools required for every step of the ML development lifecycle in one integrated, fully managed service. As a fully managed service, SageMaker removes the undifferentiated heavy lifting associated with machine learning, so you can have more time, resources and energy to solve your business problems.

You can see that for every need within a stage of the ML life cycle, SageMaker can fulfill that need. 
[Image: image.png]For preparing data, you can use Ground Truth to label data, Data Wrangler to prepare data, and Processing to run data processing and featuring engineering scripts. You can then store your features in Feature Store, and detect bias within your data with Clarify.

For building your models, you can use 18 build-in algorithms fully managed by SageMaker. Or you can bring your own scripts and even your own docker image for more customization to your model. You can use an autoML tool like Autopilot, or use pre-built solutions with JumpStart.

For training and tuning your models, you use SageMaker’s managed training to have SageMaker handle managing the infrastructure during training and automatically shut it down when complete. you can use Experiments to track your model’s lineage, Model Tuning to automatically optimize your model and Debugger to debug and profile training jobs.

Finally for deployment, you can continuously monitor your models with Model Monitor to see how your model performs over time. You can use Pipelines to build an MLOps pipeline. You can have SageMaker manage a real-time endpoint, or run batch predictions with batch transform.