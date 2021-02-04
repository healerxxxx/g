# 
export const getUrlQuery = (name, url) => {
  url = url || window.location.href
  let reg = url.match(new RegExp('[?&]' + name + '=([^?&#]*)', 'i'))
  return reg ? reg[1] : null
}
