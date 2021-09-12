<template>
        <v-app-bar
      app
      color="dark"
      dark
      dir="rtl"
       v-bind:style="styleObject"
    >
     
      <v-row
    align="center"
    justify="space-evenly"
  >
    <v-btn text>
      בית
    </v-btn>
    <v-btn text>
      עלינו
    </v-btn>
    <v-btn text>
      תוכנית לימודים
    </v-btn>
    <v-btn text>
      לקוחות מספרים
    </v-btn>  
    
  </v-row>
     
    <v-spacer></v-spacer> 
     
      <div class="d-flex align-center">
        <v-img
          alt="flashdev Logo"
          class="shrink mr-2"
          contain
          src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAZsAAAB3CAMAAADitx2HAAAAAXNSR0IB2cksfwAAAAlwSFlzAAALEwAACxMBAJqcGAAAAaRQTFRFAAAAAAAASUlJv7+/////////AAAAgICA////AAAA////7Y8D7Y8D97EY+7sf/8oo/8ooAAAAQEBA7Y8D/8oo/8ooAAAAAAAAj4+P////gICA////AAAA8JoK+LQa/sYm/8ooQEBA7Y8D+7sf/8oo/8oo/8oo7Y8D9KUR7+/v7Y8D/8ooAAAAMDAw7Y8D75YI/8oo7Y8D97AY7Y8D/8oo7Y8D8JoK////////86EP7Y8D9q0W/8oo+bYc7Y8D8JkJ86QQ7Y8Dqqqqn5+f////AAAA////////YGBg////AAAAgICAqqqq39/fubm51dXVbW1tERERz8/P////Ozs7////mZmZn5+fzMzMv7+/Tk5Or6+vFRUVAAAAAAAAEhIS39/f7u7ucHBw////AAAAEBAQ7pMF/L8h/8oo/cMj29vb7Y8D8ZsK/8oo9akT/8oo7Y8D+bgc7pQGAAAAICAgi4uL6+vrAAAAYGBgAAAA8p4Md3d3GhoagICAUFBQv7+/////6urqNzc37pMFgICA75QG+7sf+74h86MP9KUR+bYc/sUlDiaB/wAAAIx0Uk5TADBwgIAgYIBggEAQQHCAgEBAgIBgMBC/////v/+v////////758gj///n1Bw/1D/EM//MN9w/88w/7//rzAgYN9gv/+fUFAQgHAgQGCAr79w7//vz69QgJ//z/+/r+/f/+//39//7//P/9/f73D/v+//z5//r8/P/4//758g/7+Pv9//v6+/7++Av7/NtCKjAAAIFklEQVR4nO2d+WPURBSAd2WhtEXrWlwsW2EpRa4KYisURJRawFYRcV2lIBWtaBERFRXw4PA+/ml3c72ZN/MmM9lNNinv+63pJHkz32beJJkkpRLDMAzDMAzDMAzDMAzDMAzDMAzDMAzDMAzDMMwapPzYuorAevjPhoFw4cb0wxiMIhhyWm940+NPjIQ8GVO4+pSunikxCnFtfjrJBmpbnhmTEFpmy9ZwYb1X8dKMRxFUHNba9Oy27Q1gJKb44A5dPVNiYqcQ2eSu55w3AO1fRDe794hm8uymbWez4/rl8b0FdrNvT6NRGDeNxn639aeeR2qK5ObA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"
          transition="scale-transition"
          width="250"
          />

  
      </div>

    </v-app-bar>
</template>
<script>
 export default { 
     name:'header',
 
 
 data: () => ({
   styleObject:{
   
    
   }
  }),
 
 
 }
</script>

