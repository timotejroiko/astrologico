---
layout: page
title: Response - Planets
navigation: 6
---

<style>
	.inner a {
		color: royalblue;
		font-weight: bold;
	}
	.inner code {
		font-size: 100%;
	}
	.navigation li {
		padding: 0.3vh;
	}
	.sidebar {
		min-width: 300px;
	}
	.sidebar .sidebar-main {
	    height: calc(100% - 50px);
	    overflow-y: auto;
	}
	@media (max-width: 745px) {
		.sidebar .sidebar-main {
		    height: calc(100% - 320px);
		}
	}
</style>

<br>

## Planets

The planets field contains all the calculated planetary data keyed by Object IDs.

| Value | Type | Descripton |
|---|---|
| [Object ID](/astrologico/res_data.html) | Object | Object containing planetary data for the specified object |
| [Object ID](/astrologico/res_data.html) | Object | Object containing planetary data for the specified object |
| ... | Object | etc... |

For example, the ID for the Sun is `P0`, the response for the sun data will be:

```
{
	"planets": {
		"P0": {
			//planetary data for the Sun
		}
	}
}
```

<br><br><br>