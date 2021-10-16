FROM node:alpine

WORKDIR /app
COPY ./package.json ./
RUN npm install
COPY . .

ENV MONGO_URL=mongodb+srv://Aarti:aarti@zomato-master.fqdxy.mongodb.net/zomato?retryWrites=true&w=majority
ENV GOOGLE_CLIENT_ID=317097733958-jtll7v2hlg4kmuts06lle0vjrqocom2h.apps.googleusercontent.com
ENV GOOGLE_CLIENT_SECRET=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
ENV AWS_S3_ACCESS_KEY=AKIAULAZXFSDNYIJCQNH
ENV AWS_S3_SECRET_KEY=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
ENV MAILGUN__API__KEY=b3a71bd0b6229b67878f55580ff4b7c1-2ac825a1-9892eab6
ENV MAILGUN__DOMAIN=sandbox1cdb3edd99614de6a2d4a9b09592f6ef.mailgun.org
ENV RZR_PAY_ID=rzp_test_Jnh2ZBlJffiG4I
ENV RZR_PAY_SECRET=39d2ffc0f349d17d3c665fdb023ecbe2
ENV NODE_ENV=production
ENV PORT=4000

RUN npm run build


CMD ["npm", "run", "start"]