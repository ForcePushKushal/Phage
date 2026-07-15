# Phage

# Objective

# Proposed solution

# Requirements
## Tech Stack
- backend - [[FastAPI]]
- Auth - [[Supabase]]
- DB - [[Postgresql]] in Supabase
- Frontend - Vanilla JS

## Hosting
- docker
- Raspberry Pi
- Vercel

# Features
1. User profile
	1. Best 3 dishes displayed
	2. Recent foods
2. able to give reviews and ratings
3. ability to follow other users

# Plan of Execution
## Phase 1.1: setting up basic database & docker and github - 14/7/26
### User tables with authentication
#### Following table

| follow_id | follower_id | following_id | created_at |
| --------- | ----------- | ------------ | ---------- |
| INT8      | UUID        | UUID         | timestampz |

#### review table

| review_id | user_id | review_text | restaurant_name | rating | food_name | image_link | created_at |
| --------- | ------- | ----------- | --------------- | ------ | --------- | ---------- | ---------- |
| INT8      | UUID    | TEXT        | TEXT            | FLOAT8 | TEXT      |            | timestampz |

### test out basic crud functions on supabase
### Setup [[Github]]
- create a github repo, copy the ssh link
- do `git remote add origin "ssh link"` in the local project folder

## Phase 1.2: try supabase auth on fastapi

#### requirements.txt
`fastapi[standard]`- fastapi cli version: 0.0.29, cloud cli version: 0.22.2
[[Supabase]] - downloaded through [[homebrew]] - version:2.109.1 ==try to use "curl -L https://github.com/supabase/cli/releases/latest/download/supabase_linux_amd64.tar.gz -o supabase.tar.gz tar -xzf supabase.tar.gz sudo mv supabase /usr/local/bin/"==
# Future Features
1. Restaurant Pages / Food tag pages
2. Tags for cuisine, food
3. get a search option for restaurant
	1. either source it through api
	2. create database for the restaurants 
	3. data processing from user data input of restaurants
4. Picture through website

## Phase 1.2: 

# Future Features
1. Restaurant Pages / Food tag pages
2. Tags for cuisine, food
3. get a search option for restaurant
	1. either source it through api
	2. create database for the restaurants 
	3. data processing from user data input of restaurants
4. Picture through website

