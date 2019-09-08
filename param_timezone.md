---
layout: page
title: Parameters - Timezone
navigation: 5
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

## Timezone

Timezone can be manually specified using either an offset in minutes or a timezone string according to the [tz-database specification](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).

| Type | Descripton |
|---|---|
| String/Integer | Timezone string or offset minutes |

<br>

### Examples

| GET | POST | Descripton |
|---|---|---|
| `timezone=America/New_York` | `timezone:"America/New_York"` | Set timezone to America/New_York (UTC-5 or UTC-4) |
| `timezone=300` | `timezone:300` | Set timezone to +300 minutes (UTC+5) |
| `timezone=-120` | `timezone:-120` | Set timezone to -120 minutes (UTC-2) |

<br><br><br>