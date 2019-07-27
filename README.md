## To Run The Monorepo React app in docker
- docker build -t monorepo/reactapp -f ./packages/react-app/Dockerfile .
- docker run -it -p 8080:80 monorepo/reactapp
- Open http://localhost:8080/

## To run the Monorepo Next.js app in docker
- docker build -t monorepo/nextapp -f ./packages/next-app/Dockerfile .
- docker run -it -p 3000:3000 monorepo/nextapp:latest
- Open http://localhost:3000

## To run the Monorepo Gatsby.js app in docker
- yarn gatsby-build
- docker build -t monorepo/gatsbyapp -f ./packages/gatsby-app/Dockerfile .
- docker run -it -p 8080:8080 monorepo/gatsbyapp:latest
- open http://localhost:8080
