FROM node:16.9.0 AS development
ENV NODE_ENV development
# Add a work directory
WORKDIR /app
# Cache and Install dependencies
COPY package.json .
COPY yarn.lock .
RUN yarn install
# Copy app files
COPY . .
# Expose port
EXPOSE 3000
ENV CI=true
ENV HOST="localhost"
# Start the app
CMD [ "yarn", "start" ]