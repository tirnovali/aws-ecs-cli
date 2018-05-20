# AWS & ECS Useful Tips

### List AWS CLI Profiles
```
aws configure list
```

### Use Different Profiles for Commands

```
aws ec2 describe-instances --profile user2
```