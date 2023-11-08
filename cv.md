 <div style="display: flex; align-items: center;">
        <div style="flex: 0 0 auto; margin-right: 20px;">
            <img src="74094635.jpg" alt="alt text" width="250" />
        </div>
        <div>
            <h2>Hanna Pleshko</h2>
            <h3>Contact Information:</h3>
            <p>Email: anna-pleshko2000@mail.ru</p>
            <p>Phone: +375291559155</p>
            <p>Telegram: @hannapleshko</p>
            <p>LinkedIn: <a href="https://www.linkedin.com/in/hanna-p-06853a203/">My Profile</a></p>
        </div>
    </div>

## Briefly About Myself:
- About 1 year of professional experience as a FullStack JavaScript/TypeScript developer.
- Skilled in back-end development with Express, Nest, LoopBack, and front-end technologies such as
React, Redux, RTK, and RTK Query.
- Hands-on experience with client-server architectures, networking protocols, designing REST and SOAP
APIs, web services development, and database access.
- Experienced in utilizing databases like PostgreSQL, MySQL, MongoDB, IBMdb2.
- Proficiently using testing frameworks like Jest and Mocha for ensuring reliable, high-quality code
through rigorous unit tests for back-end functionality and integration tests for API endpoints.
- Skilled in deciphering existing codebases and documenting code using OpenAPI and Swagger.
- Considerable experience in object-oriented programming, implementing SOLID and REST principles,
multi-threading, concurrency, code refactoring, and thorough code reviews.
- Possess strong skills in code refactoring, reviewing, maintaining code quality, and adhering to best
practices in software development consistently

## Skills:
- Programming Languages: JavaScript, TypeScript, PHP
- Web Technologies:	Node.js, Express, React, Redux, Redux Toolkit, Redux Toolkit Query, jQuery, Bootstrap, React-Bootstrap, Material UI, Mantine, AG Grid, Mongoose, Jest, Mocha, swagger, HTML, CSS, LESS / SASS(SCSS), webpack, Babel, Bash, Docker
- Application Servers: Node.js, Apache
- Databases: PostgreSQL, MySQL, MSSQL, MongoDB, IBMdb2

## Code example:
A React component that displays a list of job vacancies, filters them based on a search string, and provides pagination for convenient navigation through the results.
```
import React, { useState, useEffect, useRef } from 'react';
import { Pagination } from '@mantine/core';
import Item from './Item';
import storage from '../../storage/storage.json';

function List({ searchString }) {
  const [list, setList] = useState(storage);
  const [currentPage, setCurrentPage] = useState(1);
  const pageSizeRef = useRef(4);

  const filterVacancy = () => {
    if (!searchString) return storage;
    return storage.filter(({ vacancy }) => vacancy.toLowerCase().includes(searchString.toLowerCase()));
  };

  const paginatedList = filterVacancy().slice((currentPage - 1) * pageSizeRef.current, currentPage * pageSizeRef.current);

  useEffect(() => {
    setList(filterVacancy());
  }, [searchString]);

  return (
    <div>
      {paginatedList.map((el, index) => (
        <Item key={index} vacancyItem={el} />
      ))}
      <Pagination
        total={Math.ceil(list.length / pageSizeRef.current)}
        value={currentPage}
        onChange={(page) => setCurrentPage(page)}
        position="center"
      />
    </div>
  );
}
```

## Work Experience
### IBA Group / Full Stack Developer / April 2022 - November 2022
CV creator for company employees. An application comprising both client and server components. The primary objective is to streamline the resume creation process for easy editing and quick completion. The product facilitates uniform CV generation, conversion to DOC format, and storage.
Responsibilities:
- Front-end and back-end development.
- Designed and optimized database schemas to ensure - efficient data storage and retrieval.
- Conducted unit tests to ensure code reliability and quality.
- Collaborated with the team in an Agile/Scrum environment to plan and execute project sprints.
- Documented APIs using OpenAPI and Swagger to ensure clear and organized documentation

### IBA Group /  Node.js Developer / September 2021 - June 2022
Application program interface (API) that allows programmers to access Microsoft Exchange items such as calendars, contacts and email.
Responsibilities:
- Back-end development.
- Collaborated with Exchange Web Server to ensure seamless integration and interaction with the API.
- Implemented middleware to validate SOAP request data
- Conducted unit tests to ensure code reliability and quality.
- Collaborated with the team in an Agile/Scrum environment to plan and execute project sprints.
- Documented APIs using OpenAPI and Swagger to ensure clear and organized documentation

### Pragma /   Full Stack Developer / February 2021 – August 2021
AMO Stock - an application tailored for amocrm, catering to individual entrepreneurs and managers who seek meticulous sales tracking and management.
Responsibilities:
- Developed and maintained the application, ensuring seamless integration with the amocrm platform.
- Collaborated with the amocrm ecosystem to ensure a unified user experience and smooth data flow.
- Collaborated with the team in an Agile/Scrum environment to plan and execute project sprints.
- Participated in code reviews to maintain code quality and adhere to best practices.

## Education
- Belarusian State University of Informatics and Radioelectronics, Faculty of Computer Design, 2022
**Courses and Certificates:** 
- NestJS Zero to Hero - Modern TypeScript Back-end Development, Udemy
- Node.js: The Complete Guide to Build RESTful APIs, Udemy
- Node.js Express - unit testing/integration tests with Jest, Udemy
- Master SOLID principles and deep dive into advanced topics in software architecture, Udemy

## English Language
English Pre-Intermediate (A2). But I'm actively improving it through courses and
interactions with international clients ;)
