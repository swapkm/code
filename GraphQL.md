
{
  postBySlug(slug: "my-new-post") {
    id
    title
    content
    createdAt
    updatedAt
    slug
  }
}

> This query will retrieve the post with the slug "my-new-post" and return its id, title, content, createdAt, updatedAt, and slug fields.



query FetchPosts($first: Int!, $after: String) {
  posts(first: $first, after: $after) {
    totalCount
    edges {
      cursor
      node {
        id
        title
        content
        slug
      }
    }
    pageInfo {
      hasNextPage
      endCursor
    }
  }
}

