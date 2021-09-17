# IAM CLI Commands

The cli commands for IAM are a bit weird because of the fact that you are editing peoples permissions. Use the below as a starting place

> Be careful not to edit users or groups that affect your access or we will have to go in with the root account and fix it

# USERS

### UPDATE

```bash
aws cloudformation deploy \
  --template-file ./IAM/Users.yaml \
  --stack-name iam-users \
  --capabilities CAPABILITY_NAMED_IAM \
  --profile realium \
  --region us-east-2
```

# GROUPS

### UPDATE

```bash
aws cloudformation deploy \
  --template-file ./IAM/Groups.yaml \
  --stack-name iam-groups \
  --capabilities CAPABILITY_NAMED_IAM \
  --profile realium \
  --region us-east-2
```
