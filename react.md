# React

## Instructions

Explain as much of this component as you can. Use line numbers and technical terms.

```js
import axios from 'axios'
import { useState, useEffect } from 'react'
import { Link, useParams, useNavigate } from 'react-router-dom'

import Reviews from './Reviews'

const API = process.env.REACT_APP_API_URL

function BookmarkDetails() {
  const { id } = useParams()
  const [bookmark, setBookmark] = useState([])
  const navigate = useNavigate()

  useEffect(() => {
    axios
      .get(`${API}/bookmarks/${id}`)
      .then((response) => {
        setBookmark(response.data)
      })
      .catch((c) => {
        console.warn('catch', c)
      })
  }, [id])

  return (
    <>
      <article>
        {bookmark.is_favorite ? <span>⭐️</span> : null} {bookmark.name}
        <h5>
          <span>
            <a href={bookmark.url}>{bookmark.name}</a>
          </span>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {bookmark.url}
        </h5>
        <h6>{bookmark.category}</h6>
        <p>{bookmark.description}</p>
        <div className="showNavigation">
          <>
            <Link to={`/bookmarks`}>
              <button>Back</button>
            </Link>
          </>
          <>
            <Link to={`/bookmarks/${bookmark.id}/edit`}>
              <button>Edit</button>
            </Link>
          </>
          <>
            <button onClick={handleDelete}>Delete</button>
          </>
        </div>
      </article>
      <Reviews />
    </>
  )
}

export default BookmarkDetails
```
