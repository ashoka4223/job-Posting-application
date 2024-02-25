
# Job Linsting Application


JobListing App

This simple job listing application allows users to both post and search for job listings. Built using MongoDB for data storage. Users can easily search for jobs by keyword, streamlining the job search process. With clean and intuitive interface design, this application offers a user-friendly experience for both employers and job seekers.


## API Reference

#### Get Swagger UI 

```http
  GET "/"
```
#### Get all posts

```http
  GET /allPosts
```


#### Get  post

```http
  GET /posts/{text}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |





## Authors

- [@ashoka4223](https://github.com/ashoka4223)


## Demo

https://drive.google.com/file/d/1O8u0fP_mSBzdqC1v6WJKToCx7711kADt/view?usp=sharing


## Run Locally

Clone the project

```bash
  git clone https://github.com/ashoka4223/job-Posting-application.git
```

Go to the project directory

```bash
  cd JobPost Backend/joblisting/
```

Configure Application.properties file according to your Database

Go to MongoDB Atlas and find this url string in Overview and tyen Connect Current IP address.

<img width="815" alt="Connect" src="https://github.com/ashoka4223/job-Posting-application/assets/112795808/295b1a9e-230a-42c8-a550-d4a4a20d701f">

After that 


<img width="815" alt="MongoDB" src="https://github.com/ashoka4223/job-Posting-application/assets/112795808/c4e4b921-66f0-4e95-9084-82cd56a82c91">


```bash
spring.data.mongodb.uri= # uri of mongoDB cluster 
spring.data.mongodb.database=   Joblisting <--database name
logging.level.org.springframework=INFO
springdoc.api-docs.path=/api-docs
```

Install dependencies

#### Save or refresh pox.xml file

Start the server

```bash
  mvn spring-boot:run
```

