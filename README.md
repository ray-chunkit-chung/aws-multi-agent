# aws-multi-agent

https://qiita.com/hayao_k/items/57cf2e7950c04e88895a

https://docs.aws.amazon.com/bedrock/latest/userguide/agent-tutorial-step5.html


```bash
aws cloudformation deploy \
  --template-file pipeline.yaml \
  --stack-name GitHubCFPipeline \
  --capabilities CAPABILITY_NAMED_IAM \
  --parameter-overrides \
    GitHubOwner=your-github-username \
    GitHubRepo=your-repo-name \
    GitHubBranch=main \
    GitHubOAuthToken=your-token
```