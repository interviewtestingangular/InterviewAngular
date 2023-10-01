## Please fill the missing lines to make this component execute

import { Component, OnInit } from '@angular/core'<br />;
{import statement missing}<br />

@Component({<br />
&emsp;&emsp;selector: 'app-user-list',<br />
&emsp;&emsp;templateUrl: './user-list.component.html',<br />
&emsp;&emsp;styleUrls: ['./user-list.component.css']<br />
})<br />

export class UserListComponent implements OnInit {<br />


constructor(private http: HttpClient) { }<br />

ngOnInit() {<br />
// Make an HTTP GET request to fetch user data from the API<br />
this.http.get<any[]>('https://api.example.com/users').subscribe(<br />
&emsp;&emsp;(response) => {<br />
&emsp;&emsp;&emsp;// Fill in the missing lines here to assign the response data to the 'users' array<br />
},
&emsp; (error) => {<br />
&emsp; &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;       console.error('Error fetching user data:', error);<br />
&emsp; &emsp;&emsp;&emsp;}<br />
&emsp;&emsp;&emsp;);<br />
&emsp;&emsp;}<br />
}