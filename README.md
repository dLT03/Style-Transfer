# CTRL + Style: Stylometry & Style Transfer with Sentence Embeddings

This project explores how literary style is encoded in sentence embeddings and investigates style transfer between literary texts from different eras (classical 19th literature vs 20th century new wave).

## Dataset
The dataset consists of 135 text fragments with metadata:
| Column          | Description                                                                |
| --------------- | -------------------------------------------------------------------------- |
| `author`        | Author of the text                                                         |
| `title`         | Title of the literary work                                                 |
| `style`         | Literary style (`XIX` or `XX`)                                             |
| `transfer_type` | Indicates whether text is original or style-transferred (`ORIGINAL`, etc.) |
| `text`          | Raw text fragment                                                          |


## Goal
- Analyze how literary style (XIX vs XX century) is reflected in sentence embeddings
- Evaluate how well style-transferred (by AI models) texts match their target style
- Visualize clustering and separation of styles using dimensionality reduction techniques
  
## Methods
- Sentence Embeddings: all-mpnet-base-v2 from sentence-transformers
- Clustering: KMeans to group similar styles
- Evaluation: Silhouette Score, accuracy, confusion matrix
- Visualization: UMAP, t-SNE, Convex Hulls for cluster shapes

## Key Findings
- Embeddings reflect meaningful stylistic differences between literary eras
- Clustering algorithms can separate styles with moderate-to-high silhouette scores
- Style transfer quality can be visually and numerically assessed
