# Users

```json
{
	"id": "string",
	"username": "string",
	"first_name": "string",
	"last_name": "string",
  	"joinedAt": "number",
	"email": "string",
	"phone": "number",
	"yoe": "number",
	"company": "string",
	"designation": "string",
	"img": "string",
	"github_id": "string",
	"github_display_name": "string",
	"linkedin_id": "string",
	"twitter_id": "string",
	"instagram_id": "string",
	"skills": [],
	"joined_discord": "string",
	"website": "string",
	"isMember": "boolean",
	"userType": "string",
  	"githubLinkedAt": "number",
	"tokens": {
		"githubAccessToken": "string"
	},
	"status": "string",
	"roles": {
		"app_owner": "boolean",
		"archived": "boolean",
		"member": "boolean",
		"restricted": "boolean",
		"super_user": "boolean",
		"in_discord": "boolean"
	},
	"profileURL": "string",
	"picture": {
		"publicId": "string",
		"url": "string"
	},
	"created_at": "timestamp",
	"updated_at": "timestamp"
}
```

### Example

```json
{
  "id": "12345",
  "username": "ankur",
  "first_name": "Ankur",
  "last_name": "Narkhede",
  "joinedAt": 1686014202464,
  "email": "abc@gmail.com",
  "phone": 1234567890,
  "yoe": 0,
  "company": "BigCo",
  "designation": "Software Engineer",
  "img": "./img.png",
  "github_id": "ankur",
  "github_display_name": "Ankur Narkhede",
  "linkedin_id": "ankurnarkhede",
  "twitter_id": "whatifiz",
  "instagram_id": "myIgId",
  "skills": [],
  "joined_discord": "2023-01-13T18:21:09.278000+00:00",
  "website": "mywebsite.com",
  "isMember": true,
  "userType": "",
  "githubLinkedAt":1686013994127,
  "tokens": {
     "githubAccessToken": "ankurGithubAccessToken",
  },
  "status": "active",
  "roles": {
    "app_owner": false,
    "archived": false,
    "member" : true,
    "restricted": false,
    "super_user": false,
    "in_discord" : true,
  },
  "profileURL": "https://abcde.com",
  "picture":{
    "publicId": "profile/mtS4DhUvNYsKqI7oCWVB/aenklfhtjldc5ytei3ar",
    "url": "https://res.cloudinary.com/realdevsquad/image/upload/v1663885133/profile/mtS4DpUvNYsKqI7oCWVB/aenklfhtjldc5ytei3ar.jpg",
  },
"created_at": 1683676800000,
"updated_at": 1683676800000

}
```
