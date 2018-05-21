# AWS & ECS Useful Tips

### List AWS CLI Profiles
```
aws configure list
```

### Use Different Profiles for Commands

```
aws ec2 describe-instances --profile user2
```

### Creating ECS CLI Configuration

- Default Launch Type : **Fargate**
- Region : **us-east-1** // Ireland
- Cluster : tutorial
- Config Name : tutorial

```
ecs-cli configure --cluster tutorial --region us-east-1 --default-launch-type FARGATE --config-name tutorial
```

### Adding ECS CLI Credentials

- Access Key
- Secret Key 
- Profile Name : tutorial

```
ecs-cli configure profile --access-key AWS_ACCESS_KEY_ID --secret-key AWS_SECRET_ACCESS_KEY --profile-name tutorial
```