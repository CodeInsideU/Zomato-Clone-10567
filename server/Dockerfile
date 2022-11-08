FROM node:alpine

WORKDIR /app
COPY ./package.json ./
RUN npm install

COPY . ./

ENV MONGO_URL = mongodb+srv://VratikZade:vratikzade@cluster0.nws17vq.mongodb.net/?retryWrites=true&w=majority
ENV JWTSECRET = ZomatoApp
ENV AWS_S3_ACCESS_KEY = AKIARXOOVFAJTFVSBFOC
ENV AWS_S3_SECRET_KEY = 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
ENV GOOGLE_CLIENT_ID = 1093757863142-2smgu18ucil1o1vkl1d1e1ti8kr3c0c3.apps.googleusercontent.com
ENV GOOGLE_CLIENT_SECRET = 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


RUN npm run build

CMD [ "npm","run","start"]
