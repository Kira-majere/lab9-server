# lab9-server
ссылка на деплой heroku:     https://immense-reaches-97039.herokuapp.com/

примеры запросов
query GetLaunchById {
  launch(id: 40) {
    id
    rocket {
      id
      type
    }
  }
}

query GetLaunchById($id: ID!) {
  launch(id: $id) {
    id
    rocket {
      id
      type
    }
  }
}   (но надо указать вариант в поле query variables   {"id": 60})
