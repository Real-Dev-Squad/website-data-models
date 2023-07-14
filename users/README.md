# Users

```json
{
	"id": "string",
	"username": "string",
	"first_name": "string",
	"last_name": "string",
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
    "archivedDetails": {
    "updated_at": "number",
    "super_user_id": "string",
    "reason": "string"
  },
	"profileURL": "string",
	"picture": {
		"publicId": "string",
		"url": "string"
	}
}
```

### Example

```json
{

  'id': string,
  'username': string,
  'first_name': string,
  'last_name': string,
  'email': string,
  'phone': number,
  'yoe': number,
  'company': string,
  'designation': string,
  'img': string,
  'github_id': string,
  'github_user_id': string,
  'linkedin_id': string,
  'twitter_id': string,
  'instagram_id': string,
  'skills': [],
  'website': string,
  'github_display_name': string,
  'isMember': boolean,
  'userType': string,
  'tokens': {},
  'status': string

  "id": "12345",
  "username": "ankur",
  "first_name": "Ankur",
  "last_name": "Narkhede",
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
    "archivedDetails": {
    "updated_at": "1689336810",
    "super_user_id": "LQBMyug9eHeC3zooncVN",
    "reason": "Officia irure laboris sit."
  },
  "profileURL": "https://abcde.com",
  "picture":{
    "publicId": "profile/mtS4DhUvNYsKqI7oCWVB/aenklfhtjldc5ytei3ar",
    "url": "https://res.cloudinary.com/realdevsquad/image/upload/v1663885133/profile/mtS4DpUvNYsKqI7oCWVB/aenklfhtjldc5ytei3ar.jpg",
  }

}
```
