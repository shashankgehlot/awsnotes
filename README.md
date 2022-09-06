**# awsnotes**
## Region
1. aws has regions all around world
2. regions are cluster of data centers
3. Most aws services are region scoped

### how do you choose aws Region?
    1. Compliance : based on govt polices -> apna data apne ghar
    2. Proximity: based on latency 
    3. Availabliy: not all regions have all services
    4. pricing : pricing varies region to region 
### Aws availablity zones
    1. Regions have availabliy zones
        usually:3
        min:2
        max:6
    2. each AZ is discrete data center with redundent power,networking,connectivity
    3. they are sepreted to each other so when disaster happens they are isolated.
    4. connected with high bandwidth ultra low latency.


### Edge location
    1. 216 points on presence in 84 city accross  42 countries 
    2. content is delivered to user with low latency.

### Iam User and Groups
    1. Iam : identity and Acess management . `Global service`
    2. Root account created by default should not be shared
    3. User are people in organization that can be grouped
    4. Group only contain User not groups
    5. A user can belong to multiple Groups, A user can not be associated with Any Group
![Alt text](./UserandGroup.png?raw=true "User and groups")
### 
    7. user and Groups can be assigned Json docs called policy.
    **docs contain permisson details of User.**
    8. Least Previlage Principle:
        dont give more permission than user needs.
![Alt text](./policies.png?raw=true "policies")

    

### Policy structure
    1. it will have version No
    2. identifier for policy
    3.Statement

    statement contains:
        >id
        >Effect: Allow/denies
        >principal: which account user/group will have this policy applied to
        >Action:list of apis which will be allowed denied
        resource: list of resources on which the action is applied to



