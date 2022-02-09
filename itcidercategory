	function replaceLink() {
    var aLink = $('a');
    for(var i=0;i<aLink.length;i++) {
        if(aLink.eq(i).attr('href')) {
            aLink.eq(i).attr('href',aLink.eq(i).attr('href').split("?category=")[0]);
        }
    }
}
	$(document).ready(function() {
    replaceLink();
});
	if (typeof(history.pushState) == 'function') {
    var CatagoryURL = location.href;
    CatagoryURL = CatagoryURL.replace(/\?category=([0-9]+)/ig, '');
    history.pushState(null, null, CatagoryURL);
}
