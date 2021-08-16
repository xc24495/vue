var axios = require("axios").default;

var options = {
  method: 'POST',
  url: 'https://google-translate20.p.rapidapi.com/translate',
  headers: {
    'content-type': 'application/x-www-form-urlencoded',
    'x-rapidapi-key': 'ae01a74d14msh2668096e270cfa0p147651jsne3efb65c0fb8',
    'x-rapidapi-host': 'google-translate20.p.rapidapi.com'
  },
  data: {
    text: 'The POST method has several advantages over GET: it is more secure because most of the request is hidden from the user; Suitable for big data operations.',
    tl: 'es',
    sl: 'en'
  }
};

axios.request(options).then(function (response) {
	console.log(response.data);
}).catch(function (error) {
	console.error(error);
});
