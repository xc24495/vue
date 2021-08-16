import axios from "axios";

const options = {
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


import axios from "axios";

const options = {
  method: 'POST',
  url: 'https://google-translate1.p.rapidapi.com/language/translate/v2',
  headers: {
    'content-type': 'application/x-www-form-urlencoded',
    'accept-encoding': 'application/gzip',
    'x-rapidapi-key': 'ae01a74d14msh2668096e270cfa0p147651jsne3efb65c0fb8',
    'x-rapidapi-host': 'google-translate1.p.rapidapi.com'
  },
  data: {q: 'Hello, world!', target: 'es', source: 'en'}
};

axios.request(options).then(function (response) {
	console.log(response.data);
}).catch(function (error) {
	console.error(error);
});
